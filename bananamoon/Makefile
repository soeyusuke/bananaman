.PHONY: glide
glide:
ifeq ($(shell which glide 2>/dev/null),)
	curl https://glide.sh/get | sh
endif

.PHONY: deps
deps: glide
	glide install

.PHONY: build
build: deps
	go build 

