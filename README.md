# geocoder.sif <a href='https://degauss.org'><img src='https://github.com/degauss-org/degauss_hex_logo/raw/main/PNG/degauss_hex.png' align='right' height='138.5' /></a>

[![.github/workflows/build.yaml](https://github.com/degauss-org/geocoder.sif/actions/workflows/build.yaml/badge.svg)](https://github.com/degauss-org/geocoder.sif/actions/workflows/build.yaml)


This is a port of the [DeGAUSS geocoder](https://github.com/degauss-org/geocoder) Docker container to an [apptainer](https://apptainer.org/) container suitable to use with apptainer or [singularity](https://github.com/sylabs/singularity) in high performance computing environoments.

## Using

After singularity or apptainer are installed and available, pull the container from the github container registry:

```sh
apptainer pull oras://ghcr.io/degauss-org/geocoder.sif:v3.3.0
```

Call the container directly as an executable with an argument of the name of the csv file with an address column named `address`:

```sh
./geocoder.sif_v3.3.0.sif my_address_file.csv
```

See the [DeGAUSS geocoder README](https://github.com/degauss-org/geocoder?tab=readme-ov-file#geocoder-) for details.
