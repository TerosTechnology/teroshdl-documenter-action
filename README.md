<p align="center">
  <a title="TerosHDL documentation" href="https://TerosTechnology.github.io/terosHDLdoc"><img src="https://img.shields.io/website.svg?label=TerosTechnology.github.io%2FterosHDLdoc&longCache=true&style=flat-square&url=http%3A%2F%2FTerosTechnology.github.io%2FterosHDLdoc%2Findex.html"></a><!--
  -->
  <a title="Join the chat at https://gitter.im/TerosHDL/community" href="https://gitter.im/TerosHDL/community"><img src="https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef"></a><!--
  -->
</p>

<p align="left">
  <img src="teroshdl_logo.png" alt="TerosHDL logo">
</p>


# TerosHDL documenter and GitHub Actions

This repository showcases several approaches for using TerosHDL Documenter in GitHub Actions. 

# Action

Using an Action is the most idiomatic and less verbose solution.

```yml
    runs-on: ubuntu-latest
    steps:

    - uses: actions/checkout@v2

    - uses: TerosTechnology/teroshdl-documenter-action@main
      with:
        args: -i ./ --recursive --out html
```

## Options

- ```args```: TerosHDL Documenter arguments. https://github.com/TerosTechnology/colibri

