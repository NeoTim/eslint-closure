# Copyright 2017 Google Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_closure//closure:defs.bzl", "closure_js_binary")
load("@io_bazel_rules_closure//closure:defs.bzl", "closure_js_library")

closure_js_library(
    name = "types",
    srcs = ["types.js"],
    deps = [],
)

closure_js_library(
    name = "config-tester",
    srcs = ["config-tester.js"],
    deps = [
        ":error-compare",
        ":types",
        "//packages/eslint-plugin-closure/lib/externs:all-externs",
        "@io_bazel_rules_closure//closure/library",
    ],
)

closure_js_library(
    name = "error-compare",
    srcs = ["error-compare.js"],
    deps = [
        ":types",
        "//packages/eslint-plugin-closure/lib/externs:all-externs",
        "@io_bazel_rules_closure//closure/library",
    ],
)
