# Definition (recipe) file for building the computational runtime environment (container) for the LuminexPipeline utility

<p>
This is the repository of the definition file or the so-called recipe file of the execution runtime environment (container) of the LuminexPipeline (https://github.com/Asimeng/LuminexPipeline), developed as part of my MSc dissertation.
This virtual environment was developed to address the challenge of numerical instability arising from different software versioning as well as the use of different computing environments. The overarching aim was to contribute to attaining analytical reproducibility of Luminex data processing. This containerised runtime environment runs on the bitnami/minideb (https://github.com/bitnami/minideb) base OS image, which is a lightweight version of Debian OS. Additionally, the development process involved the use of the multi-stage build process to further make the container lightweight.

This container can be rebuilt from this definition (recipe) file using either of the following Singularity commands:

Using the --fakeroot parameter  <br>

`singularity build --fakeroot [preferred_container_name_.sif] [this_definition_file.def]`<br>

Or if you have administrative privileges, then: 

`sudo singularity build [preferred_container_name_.sif] [this_definition_file.def]` <br>

NB: Ensure to replace the contents in [] with appropriate names and omit the [] in the actual command on the command line.
</p>
