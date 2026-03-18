load("@aspect_rules_py//py:defs.bzl", "py_binary")
load("@rules_img//img:layer.bzl", "image_layer")

py_binary(
    name = "script",
    srcs = [":main.py"],
)

image_layer(
    name = "app_layer",
    srcs = {"/app": ":script"},
)
