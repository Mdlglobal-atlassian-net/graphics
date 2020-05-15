# Utility functionalities for tf-graphics.

licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "cleanup",
    hdrs = ["cleanup.h"],
)

cc_test(
    name = "cleanup_test",
    size = "small",
    srcs = ["tests/cleanup_test.cc"],
    deps = [
        ":cleanup",
        "//testing/base/public:gunit_main",
    ],
)

py_library(
    name = "export_api",
    srcs = ["export_api.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
)

py_library(
    name = "doc",
    srcs = ["doc.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
)

py_library(
    name = "test_case",
    srcs = ["test_case.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        ":tfg_flags",
        # "//third_party/py/absl/flags",
        # "//third_party/py/absl/testing:parameterized",
        # "//third_party/py/numpy",
        # "//third_party/py/tensorflow",
    ],
)

py_library(
    name = "tfg_flags",
    srcs = ["tfg_flags.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    # deps = [
    #     "//third_party/py/absl/flags",
    # ],
)

py_library(
    name = "type_alias",
    srcs = ["type_alias.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    # deps = [
    #     "//third_party/py/numpy",
    #     "//third_party/py/tensorflow",
    #     "//third_party/py/typing",
    # ],
)

py_library(
    name = "asserts",
    srcs = ["asserts.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        # "//third_party/py/absl/flags",
        # "//third_party/py/numpy",
        # "//third_party/py/tensorflow",
        ":tfg_flags",
    ],
)

py_library(
    name = "safe_ops",
    srcs = ["safe_ops.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        ":asserts",
        # "//third_party/py/numpy",
        # "//third_party/py/tensorflow",
    ],
)

py_library(
    name = "shape",
    srcs = ["shape.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    # deps = [
    #     "//third_party/py/six",
    #     "//third_party/py/tensorflow",
    # ],
)

py_library(
    name = "util",
    srcs = ["__init__.py"],
    srcs_version = "PY2AND3",
    #strict_deps = True,
    deps = [
        ":asserts",
        ":doc",
        ":export_api",
        ":safe_ops",
        ":shape",
        ":test_case",
        ":tfg_flags",
    ],
)
