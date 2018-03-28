workspace(name = "rxjs")

####################################
# Fetch and install the NodeJS rules
http_archive(
    name = "build_bazel_rules_nodejs",
    url = "https://github.com/bazelbuild/rules_nodejs/archive/0.6.0.zip",
    strip_prefix = "rules_nodejs-0.6.0",
)

load("@build_bazel_rules_nodejs//:defs.bzl", "node_repositories", "yarn_install")

node_repositories(package_json = ["//:package.json"])


####################################
# Fetch and install the TypeScript rules
http_archive(
    name = "build_bazel_rules_typescript",
    url = "https://github.com/bazelbuild/rules_typescript/archive/df4a1a561d88e187438ac7791a5ac33995f2d317.zip",
    strip_prefix = "rules_typescript-df4a1a561d88e187438ac7791a5ac33995f2d317",
    sha256 = "51a84f156eeddf126e9370b5c193b4709eeb330448e2de5afcda40232e0b56bc",
)

load("@build_bazel_rules_typescript//:defs.bzl", "ts_setup_workspace")

ts_setup_workspace()
