

cc_library(
    name = "mediapipeface",
    srcs = ["MediaPipeFace.cpp"],
    hdrs = ["MediaPipeFace.hpp"],
    deps =  [    
                "//third_party:opencv",
                "//graphs:face_renderer",
                "@com_google_mediapipe//mediapipe/graphs/face_mesh:desktop_live_calculators",
                "@com_google_mediapipe//mediapipe/framework:calculator_framework",
                "@com_google_mediapipe//mediapipe/framework/port:parse_text_proto"
            ],
)

cc_binary(
    name = "main",
    srcs = ["main.cpp"],
    deps = [
        ":mediapipeface",
        "//third_party:opencv",
        "@com_google_absl//absl/flags:flag",
        "@com_google_absl//absl/flags:parse",
        ],
    visibility = ["//visibility:public"],
)
