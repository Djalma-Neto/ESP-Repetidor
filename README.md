# ESP-Repetidor
Repetidor de sinal wi-fi com esp32


FONTE YOUTUBE: https://www.youtube.com/watch?v=WOMy0lWc_pM&ab_channel=MaxDicas
FONTE GITHUB: https://github.com/martin-ger/esp32_nat_router

![Alt text](./Configurações.png?raw=true "Configurações")

passo 1:
Execute o programa "flash_download_tools_v3.6.8.exe"
selecione os primeiros tres checkBox como na imagem1, logo depois em cada um adicione os arquivos "bootloader.bin @ 0x1000","esp32_nat_router.bin @ 0x10000" e "partitions_example.bin @ 0x8000" respectivamente como na imagem, verifique as configurações:
- SPI SPEED: 40MHz
- SPI MODE: DIO
- FLASH SIZE: 32Mbit

Logo depois selecione a porta em que seu ESP esta conectado , ex: COM4, para finalizar selecione a opção "START" e espere ate que finalize, reinicie o dispositivo(ESP32) verifique as redes wi-fi disponíveis e percebera que existe uma nova rede (O nome será diferente).

![Alt text](./Wi-fi.png?raw=true "Configurações")

Conecte-se a ela e acesse, atravez do navegador, o endereço 192.168.4.1 para entrar no painel de configurações do esp, la sera adicionado o SSID da rede que será repetida e o password, logo abaixo devera escolher o novo SSID e password dessa nova rede apos persistir esses novos dados o dispositivo será reiniciado e as alterações já estarão em uso.

![Alt text](./Acesso.png?raw=true "Configurações")


