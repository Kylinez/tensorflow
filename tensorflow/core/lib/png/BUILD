load(
    "//tensorflow/core/platform:rules_cc.bzl",
    "cc_library",
)

package(
    default_visibility = [
        # tensorflow/core:lib effectively exposes all targets under tensorflow/core/lib/**
        "//tensorflow/core:__pkg__",
    ],
    licenses = ["notice"],  # Apache 2.0
)

cc_library(
    name = "png_io",
    srcs = ["png_io.cc"],
    hdrs = ["png_io.h"],
    deps = [
        "//tensorflow/core/platform:byte_order",
        "//tensorflow/core/platform:logging",
        "//tensorflow/core/platform:png",
        "//tensorflow/core/platform:stringpiece",
        "//tensorflow/core/platform:types",
        "@com_google_absl//absl/base",
        "@zlib",
    ],
)

alias(
    name = "testdata",
    actual = "//tensorflow/core/lib/png/testdata:png_testdata",
    visibility = ["//tensorflow/core:__pkg__"],
)
