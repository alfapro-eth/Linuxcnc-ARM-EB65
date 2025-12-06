### Встановлення компонента Remora

Компонент Remora є інтерфейсом між LinuxCNC і платою контролера, а також відповідає за генератори крокових імпульсів зі сторони LinuxCNC. Інсталяція Remora для LinuxCNC містить кілька окремих компонентів.
Щоб встановити компонент Remora:
* Відкрийте вікно терміналу, завантажте репозиторій Remora
* Перейдіть до каталогу компонентів Remora.
* Встановіть компонент SPI
> Для BTT Octopus V1.1 використовується SPI

```bash
mkdir ~/linuxcnc
cd ~/linuxcnc
```
```bash
git clone https://github.com/alfapro-eth/Linuxcnc-ARM-EB65
```
```bash
cd Linuxcnc-ARM-EB65/Components_Remora/Remora-spi
```
```bash
sudo halcompile --install ./Remora-spi/remora-spi.c
```
