package(
    default_visibility = [
        "//visibility:public",
    ],
)

licenses(["notice"])  # Apache 2.0

cc_library(
    name = "any",
    hdrs = ["any.h"],
    srcs = ["any.cc"],
    deps = ["//cub/dci"],
)

cc_test(
    name = "any_test",
    srcs = ["any_test.cc"],
    deps = [
        ":any",
        "@xunit_cut//:cut",
        "@xunit_cut//:cut_main",        
    ],
)

cc_library(
    name = "assertions",
    hdrs = ["assertions.h"],
    deps = [
        ":status",
        "//cub/log",      
    ],    
)

cc_library(
    name = "comparator",
    hdrs = ["comparator.h"],
)

cc_library(
    name = "fwddecl",
    hdrs = ["fwddecl.h"],
)

cc_library(
    name = "inplace",
    hdrs = ["inplace.h"],
    srcs = ["inplace.cc"],
)

cc_library(
    name = "default",
    hdrs = ["default.h"],
)

cc_library(
    name = "keywords",
    hdrs = ["keywords.h"],
    deps = [":default"],
)

cc_library(
    name = "optional",
    hdrs = [
        "optional.h",
        "inplace.h"
    ],
    srcs = ["optional.cc"],    
    deps = [":placement"],
)

cc_test(
    name = "optional_test",
    srcs = ["optional_test.cc"],
    deps = [
        ":optional",
        "@xunit_cut//:cut",
        "@xunit_cut//:cut_main",        
    ],
)

cc_library(
    name = "placement",
    hdrs = ["placement.h"],
)

cc_test(
    name = "placement_test",
    srcs = ["placement_test.cc"],
    deps = [
        ":placement",
        "//cub/algo:loop",
        "//cub/dci",      
        "@xunit_cut//:cut",
        "@xunit_cut//:cut_main",        
    ],
)

cc_library(
    name = "ref_counter",
    hdrs = [
        "ref_counter.h",
        "scoped_unref.h",        
    ],
    srcs = [
        "ref_counter.cc",
        "scoped_unref.cc",            
    ],
    deps = [
        ":uncloneable",
    ],
)

cc_test(
    name = "ref_counter_test",
    srcs = ["ref_counter_test.cc"],
    deps = [
        ":ref_counter",   
        "@xunit_cut//:cut",
        "@xunit_cut//:cut_main",        
    ],
)

cc_library(
    name = "static_assert",
    hdrs = ["static_assert.h"],
)

cc_library(
    name = "status",
    hdrs = ["status.h"],
)

cc_library(
    name = "scoped_exit",
    hdrs = ["scoped_exit.h"],
    deps = [
      ":symbol",
    ],
)

cc_library(
    name = "struct_wrapper",
    hdrs = ["struct_wrapper.h"],
    deps = [
        ":static_assert",
    ],
)

cc_test(
    name = "struct_wrapper_test",
    srcs = ["struct_wrapper_test.cc"],
    deps = [
        ":struct_wrapper",
        "@xunit_cut//:cut",
        "@xunit_cut//:cut_main",        
    ],
)

cc_library(
    name = "symbol",
    hdrs = ["symbol.h"],
)

cc_library(
    name = "uncloneable",
    hdrs = ["uncloneable.h"],
)

cc_library(
    name = "hash",
    hdrs = ["hash.h"],
)
