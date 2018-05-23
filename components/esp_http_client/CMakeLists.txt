set(COMPONENT_SRCDIRS . lib)
set(COMPONENT_ADD_INCLUDEDIRS include)
set(COMPONENT_PRIV_INCLUDEDIRS lib/include)

set(COMPONENT_REQUIRES)
set(COMPONENT_PRIV_REQUIRES tcpip_adapter nghttp)

register_component()
