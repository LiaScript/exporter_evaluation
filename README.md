# LiaScript Exporter evalution

This project provides an automated export mechanism for LiaScript documents and illustrates the current state of the exporter implementation. A Github Action generates `json`, `scorm1.2` and webpages base on all LiaScript files locate in repository root. The output is available in `export`.

General information about LiaScript can be found on [Project Website](https://liascript.github.io/) or in [user documentation](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaScript/docs/master/README.md#1).


Examples
=====================

| Filename                | Interactive                                                                                                                                   | pdf                                                                                                                         |  SCORM1.2    | website                                                                                                              |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --- | -------------------------------------------------------------------------------------------------------------------- |
| `00_Basic_Markdown.md`  | [LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaScript/exporter_evaluation/main/00_Basic_Markdown.md#1)  | [Link](https://raw.githubusercontent.com/LiaScript/exporter_evaluation/main/export/00_Basic_Markdown/00_Basic_Markdown.pdf) |     | [Link](https://github.com/LiaScript/exporter_evaluation/raw/main/export/00_Basic_Markdown/00_Basic_Markdown_web.zip) |
| `01_Executable_Code.md` | [LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaScript/exporter_evaluation/main/01_Executable_Code.md#1) |   [Link](https://raw.githubusercontent.com/LiaScript/exporter_evaluation/main/export/01_Executable_Code/01_Executable_Code.pdf)                                                                                                                          |     |    [Link](https://github.com/LiaScript/exporter_evaluation/raw/main/export/01_Executable_Code/01_Executable_Code_web.zip)                                                                                                                  |

> __Currently, we improve the export functions. If you identify a problem or an interesting feature, do not hesitate to contact us. Just initiate an Issue here in Github.__


Implementation
=====================

The different export functions are activated by publishing a new version of a `md` File into this folder. Within a Github-Action a script generates a clone of the repo, extracts actual content and activates the generation process. All resulting files are stored in a `export` folder at the end.

![Image](https://www.plantuml.com/plantuml/png/dTF1QeD040RW-px5tALAhpt591OA8GQJ70gXO7LRBD4DxYPjOH--SQXkM7zxw10yVCC_OLntfatUcdDz56Lbybm8wYku6rS0dJikQ6bS3z2vytVm0fqx7CpaIUdAgFQRN2sEgf5KDHGNfbBDuCdNIRL6bhIgygKgz9K4JLMMRDBjqoxDdX_JrJB9Uj_iisIHxhFjzRdU9UjTDoFmtn8NPkIYsp8CGohku_djoeY1SpuEwz9_bO2nyuGvdk0pyc43aFSPEUSZoIVavo5xBv7pH54C_X-mQueUu_1Kldb1m2ZueLK3WXwxvZy-6NTEl_L2exAi_0GjkWbRT4NT3zzHVFa3ddOPpsH4DopoHnp8OiTvI--oaMrkv00M-rHU4H-D0zwhSrsejdPEqnFugt0m-ATyrPMHFOp31t_DQCh5J3RbkJx-0000)
