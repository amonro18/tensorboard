load("//tensorboard/defs:web.bzl", "tf_web_library")
load("//tensorboard/defs:defs.bzl", "tensorboard_webcomponent_library")

package(default_visibility = ["//tensorboard:internal"])

licenses(["notice"])  # Apache 2.0

tf_web_library(
    name = "tf_hparams_backend",
    srcs = [
        "tf-hparams-backend.html",
    ],
    path = "/tf-hparams-backend",
    deps = [
        "//tensorboard/components/tf_backend",
    ],
)

tensorboard_webcomponent_library(
    name = "legacy",
    srcs = [":tf_hparams_backend"],
    destdir = "tf-hparams-backend",
    deps = [
        "//third_party/tensorboard/components/tf_backend:legacy",
    ],
)
