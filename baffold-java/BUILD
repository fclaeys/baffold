load("@io_bazel_rules_docker//java:image.bzl", "java_image")

java_library(
    name = "server",
    srcs = glob(["src/main/java/server/Server.java"]),
    deps = [],
    visibility = ["//visibility:public"],
)

java_image(
    name = "baffold-java",
    main_class = "server.Server",
    runtime_deps = [
        ":server",
    ],
)
