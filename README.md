# bioconductor-container
Singularity container with some useful bioconductor software

## Getting Started

Clone the repository 
```
git clone https://github.com/rpolicastro/singularity.git
```

Download the container
```
singularity pull shub://rpolicastro/bioconductor-container
```

Activate the container
```
singularity shell \
-e -c \
-B directory1, directory2, ... \
bioconductor-container_latest.sif
```

The -B option lets you specify the directories you will be working with in a comma separated format.
