set(COMPONENT_ADD_INCLUDEDIRS port/include mbedtls/include)
set(COMPONENT_SRCDIRS mbedtls/library port)
set(COMPONENT_OBJEXCLUDE mbedtls/library/net_sockets.o)
set(COMPONENT_REQUIRES lwip)

register_component()

target_compile_definitions(mbedtls PUBLIC
    -DMBEDTLS_CONFIG_FILE="mbedtls/esp_config.h"
)
