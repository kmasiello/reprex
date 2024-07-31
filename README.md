## Issue
The following code fails with the output shown below:

```
> rsconnect::writeManifest()
Error in `quartoInspect()` at rsconnect/R/appMetadata-quarto.R:11:3:
! Failed to run `quarto inspect` against your content:
ERROR: /Users/katie/Desktop/reprex/.Rprofile is not a valid Quarto input document

Stack trace:
at inspectConfig
(file:///Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto.js:98794:19)
at async Command.fn
(file:///Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto.js:98808:20)
at async Command.execute
(file:///Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto.js:8104:13)
at async quarto
(file:///Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto.js:115002:5)
at async file:///Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto.js:115020:9
Run `rlang::last_trace()` to see where the error occurred.
```


## Session Info
```
> sessionInfo()
R version 4.4.0 (2024-04-24)
Platform: aarch64-apple-darwin20
Running under: macOS Sonoma 14.5

Matrix products: default
BLAS:   /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libBLAS.dylib 
LAPACK: /Library/Frameworks/R.framework/Versions/4.4-arm64/Resources/lib/libRlapack.dylib;  LAPACK version 3.12.0

locale:
[1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8

time zone: America/Los_Angeles
tzcode source: internal

attached base packages:
[1] stats     graphics  grDevices datasets  utils     methods   base     

loaded via a namespace (and not attached):
[1] compiler_4.4.0 tools_4.4.0    yaml_2.3.10    renv_1.0.7    
```