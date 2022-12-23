.PHONY: generate
generate:
	rm -rf ./go/flow/access ./go/flow/execution ./go/flow/entities ./go/flow/legacy && buf generate
	buf build -o envoy/image.pb

.PHONY: format
format:
	find ./flow/ -name "*.proto" | xargs clang-format -style=google -i
