#Angular cli

For more information about the Angular cli see https://github.com/angular/angular-cli

##Building
`docker build -t angular-cli .`

##Running
```bash
ng() {
	docker run --rm -it \
		-m 2048m \
		-v ${HOME}:${HOME}:rw \
		-w ${PWD} \
		-p 4200:4200 \
		-p 49152:49152 \
		angular-cli "$@"
}
```