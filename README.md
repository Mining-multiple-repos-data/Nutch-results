# Nutch-results
##The artifacts generated by applying proposed approach on the two versions of Nutch (open source web crawler)
*nutch.logstashed.v1 and nutch.logstashed.v2* - Nutch execution logs for version1 and version2 after logstashing

*gitdiff.txt* - git diff between the two Nutch versions that is, before and after NUTCH-1934 patch commit. Here, the SHA key is: 1. 2d84fc4a93b9866557836ae4e9db286ac8b12eba (before refactoring), and 2. 473add00cd38019e7185639dfd0ac910a25dc6cd (after refatoring)

*v2templates.txt* - Templates derived from the source code for version2

*v1templates.txt* - Templates derived from the source code for version1 by incorporating gitdiff in v2templates.txt

*notsubset.combined.txt and notmapped.combined.txt* - Set of execution log lines which are not templatized using source code templates

*templates.lex.combined.notmapped and templates.lex.combined.notsubset* - Templates generated after clustering the non templatized log lines

*logrecords.modelmining.v1.txt* - Templatized execution log file for mining execution behavior model for version1

*logrecords.modelmining.v2.txt* - Templatized execution log file for mining execution behavior model for version2

*delta_mappings.csv* - Map the inconsistent templates between version1 and version2 using multimodal approach

*vicinity.ebm.v1.json* - Discover the flow relationship between the templates for version1 that is, execution behavior for version1

*vicinity.ebm.v2.json* - Discover the flow relationship between the templates for version2 that is, execution behavior for version2

*vicinityebmdiff.json* - Identify the differences between the execution behavior model of two versions

*EBM-diff.pdf* - Execution behavior model, a graphical representation where dashed corresponds to deleted in v2, double encircled/bold corresponds to added in v2, and grey(light) corresponds to graph common in v1 and v2

*EBM-diff-annotated.pdf* - Execution behavior model differnce is annotated to highlight the potential bugs

*ebmdiff.docx* - Execution behavior model differences are analyzed to detect the potential bugs
