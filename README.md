# quickstart-se

Sample Helidon SE project that includes multiple REST operations.

## Build and run


```bash
docker build -t helidon/demo-thinjar . -f Dockerfile
```

```bash
docker build -t helidon/demo-fatjar . -f Dockerfile.fatjar
```

```bash
sed -i "s/^[#]*\s*app.greeting=.*/app.greeting=Bonjour/" src/main/resources/application.properties
```

docker run --rm -p 8080:8080 helidon/demo-fatjar:latest