# Getting Started

A guide on creating production-ready ReactJs container images without the use of a Dockerfile.

## Prerequisites

- [Docker](https://www.docker.com/)
- [Pack](https://buildpacks.io/docs/tools/pack/)
- [ReactJS](https://react.dev/)

### Step 1: Clone the repository

```
git clone https://github.com/rijkerd/oci-react-js
```

### Step 2: Build Image

```
pack build oci-react-js --builder=paketobuildpacks/builder:base --descriptor nginx.toml
```

### Step 3: Verify Image

```
docker images | grep oci-react-js
```

### Step 4: Run Image

```
docker run -d -p 8080:8080 oci-react-js
```

## Step 5: Test the Application

- [Open browser](http://localhost:8080)

## Contribute

If you encounter any problems, please don't hesitate to report them by raising an issue.

## References
