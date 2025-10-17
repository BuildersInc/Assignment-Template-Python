# Lab: Heuristic Search

## Use docker tools

```sh
# Build latex container
cd dockerfiles
docker build -t latex-builder -f latex.Dockerfile .

# Use it inside the documentation folder
cd documentation
docker run --rm -v $(pwd):/workspace latex-builder
```

## install codebase

```sh
# Build latex container
python3 -m venv .env
source ./.env/bin/activate
pip install -e .

# Run the core script
python3 -m heuristic_lab

```
