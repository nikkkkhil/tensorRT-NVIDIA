
cc_library(
    name = "cuda",
    srcs = glob([
        "src/**/*.cc",
        "src/**/*.h",
    ]),
    hdrs = glob([
        "include/**/*.h",
    ]),
    deps = [
        "//tensorrt-laboratory/core",
        "@local_config_cuda//:cuda_headers",
        "@local_config_cuda//:cuda_runtime",
    ],
    linkopts = [
        "-L/usr/local/cuda/lib64/stubs",
    ],
    strip_include_prefix = "include",
    visibility = ["//visibility:public"],
)
