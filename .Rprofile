if (!require("breakerofchains")) pak::pak("MilesMcBain/breakerofchains")
if (!require("codegrip")) pak::pak("lionel-/codegrip")

conflicted::conflict_prefer("filter", "dplyr", quiet = FALSE)
conflicted::conflict_prefer("select", "dplyr", quiet = FALSE)

options(
  download.file.method = "libcurl",
  warnPartialMatchArgs = TRUE,
  warnPartialMatchDollar = TRUE,
  warnPartialMatchAttr = TRUE
)
