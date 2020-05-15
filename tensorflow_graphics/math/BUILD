# Math functionalities for tf-graphics.

licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

py_library(
    name = "math",
    srcs = [
        "__init__.py",
    ],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    visibility = ["//visibility:public"],
    deps = [
        ":math_helpers",
        ":spherical_harmonics",
        ":vector",
        "//tensorflow_graphics/math/interpolation",
        "//tensorflow_graphics/math/optimizer",
        "//tensorflow_graphics/util:doc",
        "//tensorflow_graphics/util:export_api",
    ],
)

py_library(
    name = "vector",
    srcs = ["vector.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        #"//third_party/py/tensorflow",
        "//tensorflow_graphics/util:asserts",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:shape",
    ],
)

py_library(
    name = "spherical_harmonics",
    srcs = ["spherical_harmonics.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        ":math_helpers",
        ":vector",
        # "//third_party/py/numpy",
        # "//third_party/py/tensorflow",
        "//tensorflow_graphics/util:asserts",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:shape",
    ],
)

py_library(
    name = "math_helpers",
    srcs = ["math_helpers.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        # "//third_party/py/numpy",
        # "//third_party/py/tensorflow",
        "//tensorflow_graphics/util:asserts",
        "//tensorflow_graphics/util:export_api",
        "//tensorflow_graphics/util:safe_ops",
        "//tensorflow_graphics/util:shape",
    ],
)
