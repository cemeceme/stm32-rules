

subinclude("//build_defs:stm32")


stm32_proj(
 name="STM32_test_proj",
 ioc="TestProject.ioc",
 srcs={"Src": glob("Src/*.cpp", allow_empty = True), "Inc": glob("Inc/*.cpp", allow_empty = True)},
 cpp=True,
 visibility = ["PUBLIC"]
)

genrule(
 name="test",
 cmd="",
 srcs=[":STM32_test_proj|c_srcs"]
)

stm32_CC_library(
 name="STM32_test_cc_lib",
 ioc="TestProject.ioc",
 srcs={"Src": glob("Src/*.cpp", allow_empty = True), "Inc": glob("Inc/*.cpp", allow_empty = True)},
 visibility = ["PUBLIC"]
)
