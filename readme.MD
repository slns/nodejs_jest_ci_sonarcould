### To run sonar-scanner
Run

```bash
./install-sonar-scanner.sh
```

Go to conf/sonar-scanner.properties and uncomment below lines

```bash
sonar.host.url=http://localhost:9000
sonar.sourceEncoding=UTF-8
```

Add the bin folder path of sonar scanner in the Environment path of ubuntu by following commands

```bash
gedit ~/.profile
export PATH=”$PATH:/var/opt/sonar-scanner-4.7.0.2747-linux/bin”
```

Logout and login again to set the path

sonar-scanner -h


### To generate eslint output as per the .eslintrc file

```bash
npm run lint — -f json -o report.json
```