#Angular cli

For more information about the Angular cli see https://github.com/angular/angular-cli

##Building
`docker build -t angular-cli .`

##Running
```bash
aws() {
	docker run --rm -it \
		-m 2048m \
		-v ${HOME}:${HOME}:rw \
		-w ${PWD} \
		angular-cli "$@"
}
```