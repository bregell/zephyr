zephyr_include_directories(.)

if(CONFIG_SOC_MCIMX7_M4)
zephyr_sources_ifdef(CONFIG_CLOCK_CONTROL_IMX_CCM   ccm_imx7d.c)
zephyr_sources_ifdef(CONFIG_CLOCK_CONTROL_IMX_CCM   ccm_analog_imx7d.c)
endif()

zephyr_sources_ifdef(CONFIG_UART_IMX                uart_imx.c)
zephyr_sources_ifdef(CONFIG_GPIO_IMX                gpio_imx.c)
