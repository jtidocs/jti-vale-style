# jti-vale-style
A Vale style suitable for JTI documentation projects.

> NOTE: This project is not maintained or endorsed by [errata-ai](https://github.com/errata-ai/).


## Install

Use one of the following approaches:

1. **Manual install**:

   1. Download the [latest release](https://github.com/jtidocs/jti-vale-style/releases/tag/latest).
   2. Copy the `JTI` folder to your Vale `StylesPath`. 
   3. Include the `JTI` style in your `vale.ini` configuration file:

      ```
      StylesPath = path/to/some/directory
      MinAlertLevel = warning # suggestion, warning or error

      # Only Asciidoc and .txt files; change to whatever you're using.
      [*.{adoc,txt}]
      BasedOnStyles = JTI
      ```

2. **Package install**:
   1. Add the repo URL to your Vale `Packages` setting in your `.vale.ini` configuration file:
      ```
      StylesPath = path/to/some/directory
      MinAlertLevel = warning # suggestion, warning or error

      Packages = Google, \
      https://github.com/jtidocs/jti-vale-style/releases/download/latest/JTI.zip

      # Only Asciidoc and .txt files; change to whatever you're using.
      [*.{adoc,txt}]
      BasedOnStyles = JTI
      ```
   2. Run `vale --config path/to/vale.ini sync`