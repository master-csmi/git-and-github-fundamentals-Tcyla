# CI/CD with Git and Gitlab

## Version Control

### Merge

### 

## CI/CD Concepts

### Continuous Integration

### Continuous Delivery

### Continuous Deployment

## Gitlab Pipelines

### Basic Pipelines

```mermaid
graph Basic Pipeline;
  Build --> build_foo;
  Build --> build_bar;
  build_foo --> Test;
  build_bar --> Test;
  Test --> test_foo;
  Test --> test_bar;
```

```yml
stages:
   - build
   - test

image: basic

build_foo:
   stage: build
   script:
	- echo "building foo"

build_bar:
   stage: build
   script:
        - echo "building bar"

test_foo:
   stage: build
   script:
	- echo "testing bar"

test_foo:
   stage: build
   script:
        - echo "testing bar"

```

### Pipeline efficiency


