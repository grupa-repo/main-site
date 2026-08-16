# Grupa marketing site — https://grupa.app
#
# Requires Ruby + Bundler. Everything runs through `bundle exec` so the
# pinned Jekyll version in Gemfile.lock is the one that builds.

PORT    ?= 4000
HOST    ?= 127.0.0.1
BUNDLE  ?= bundle
# Empty for a custom domain. CI passes the repo subpath when the site is
# still deploying to github.io.
BASEURL ?=

.DEFAULT_GOAL := help
.PHONY: help start build check clean deps

help: ## Show this help
	@grep -E '^[a-z-]+:.*?## ' $(MAKEFILE_LIST) \
	  | awk -F':.*?## ' '{printf "  \033[1m%-8s\033[0m %s\n", $$1, $$2}'

start: deps ## Serve locally with live reload and open the browser
	$(BUNDLE) exec jekyll serve --host $(HOST) --port $(PORT) --livereload --open-url

build: deps ## Production build into _site/
	JEKYLL_ENV=production $(BUNDLE) exec jekyll build --baseurl '$(BASEURL)'

check: build ## Fail if unfilled legal placeholders would ship
	@if grep -rl 'SET THIS' _site >/dev/null 2>&1; then \
	  echo 'Unfilled legal placeholders in:'; \
	  grep -rl 'SET THIS' _site | sed 's|^|  |'; \
	  echo 'Fill in the legal: block in _config.yml before publishing.'; \
	  exit 1; \
	fi
	@echo 'OK — no placeholders in _site/'

clean: ## Remove build output and caches
	$(BUNDLE) exec jekyll clean

deps:
	@$(BUNDLE) check >/dev/null 2>&1 || $(BUNDLE) install
