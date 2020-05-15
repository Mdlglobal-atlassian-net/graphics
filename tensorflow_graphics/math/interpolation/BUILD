# Interpolation functionalities for tf-graphics.

licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

py_library(
    name = "interpolation",
    srcs = [
        "__init__.py",
    ],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    visibility = ["//visibility:public"],
    deps = [
        ":bspline",
        ":slerp",
        ":weighted",
        "//tensorflow_graphics/util:export_api",
    ],
)

py_library(
    name = "slerp",
    srcs = ["slerp.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        # "//third_party/py/enum",
        # "//third_party/py/tensorflow",
        "//tensorflow_graphics/math:vector",
        "//tensorflow_graphics/util:asserts",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:safe_ops",
        "//tensorflow_graphics/util:shape",
    ],
)

py_library(
    name = "bspline",
    srcs = ["bspline.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        # "//third_party/py/enum",
        # "//third_party/py/tensorflow",
        "//tensorflow_graphics/util:asserts",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:shape",
    ],
)

py_library(
    name = "weighted",
    srcs = ["weighted.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        # "//third_party/py/tensorflow",
        "//tensorflow_graphics/math:vector",
        "//tensorflow_graphics/util:asserts",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:safe_ops",
        "//tensorflow_graphics/util:shape",
    ],
)

py_library(
    name = "trilinear",
    srcs = [
        "trilinear.py",
    ],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        # "//third_party/py/tensorflow",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:shape",
    ],
)
