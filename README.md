# Ryzentosh

> This is my personal Ryzentosh build :smile:

- [Ryzentosh](#ryzentosh)
  - [Disclaimer](#disclaimer)
  - [Step by step](#step-by-step)
    - [OS X 10.15.6](#os-x-10156)
    - [Windows 10](#windows-10)
  - [Hardware specification](#hardware-specification)
    - [Benchmarks](#benchmarks)
      - [Cinebench](#cinebench)

## Disclaimer

The purpose of this project is to document the steps that to get my setup up and running. All this content can be found in any online research.

Many thanks to [Technolli][technolli] for providing such a great content out there so many can benefit from your work :clap:

## Step by step

### OS X 10.15.6

1. The first challenge was to find out what hardware parts were compatible. After doing some research, I came up with a bunch of components that would do the trick and fit my budget. The final list can be found [here](https://github.com/cirocfc/Ryzentosh/blob/master/README.md#Hardware-specification).

2. In order to install Mac OS X, I had to download it and install on a flash drive.

3. Then begun the saga of creating the EFI in the flash drive for my setup. I tried many configs, but ended up finding a built one from [Technolli][technolli] that was made for an similar setup and worked great for me \o/ This EFI setup can be found [here][efi].

4. So far so good. It took changing the BIOS settings according to [this tutorial][bios] and boot on the installation flash drive.

5. Then I formatted my Kingston SSD to APFS with GUID and started the installation process.

6. After rebooting and finishing the installation, it was necessary to mount the EFI partition on my SDD and copy the the EFI folder into the mounted partition. I used [Clover Configurator][clover] to do it.

7. Then using GenSMBIOS I activated my device (iMacPro1,1).

8. And that was it!

### Windows 10

1. First thing was to disconnect my Kingston SDD so I don't mess up with it.

2. Then I installed Windows on the Gigabyte SDD NVMe M.2.

3. The only significant change in the process here is that the Broadcom Wi-Fi card is not recognized automatically, so I had to download it from the Fenvi's website and install it using an USB drive. Even if the installation of the Bluetooth drive fails at the end of the install wizard, the card works, so don't worry.

4. And that was it!

## Hardware specification

| Component    | Link                                                                  |
| ------------ | --------------------------------------------------------------------- |
| Processor    | [AMD Ryzen 9 3900X 64MB Cache 3.8GHz 12 Cores 24 Threads][processor]  |
| GPU          | [AMD Radeon Sapphire Pulse 5700 XT BE][gpu]                           |
| Motherboard  | [Gigabyte Aorus B450 I Pro Wi-Fi AM4 Mini-iTX][motherboard]           |
| SSD NVME M.2 | [Gigabyte SDD PCI-e NVMe M.2 256 GB][nvme]                            |
| SSD Sata     | [Kingston SDD 2.5" 120 GB SATA 2][ssd]                                |
| RAM Memory   | [Hyper X Fury 16 GB RAM DDR4 2666 MHz][ram]                           |
| Power Supply | [EVGA 700w ATX 80 Plus White PFC+][power]                             |
| Wi-Fi + BT   | [Broadcom BCM94360NG Wi-Fi Dual Band + Bluetooth 4.0 PCI-e M.2][wifi] |
| Case         | [Cougar QBX Mini Tower (Mini-iTX)][case]                              |

[processor]: https://www.kabum.com.br/produto/102434/processador-amd-ryzen-9-3900x-cache-64mb-3-8ghz-4-6ghz-max-turbo-am4-sem-video-100-100000023box
[motherboard]: https://www.kabum.com.br/produto/103414/placa-mae-gigabyte-aorus-b450-i-aorus-pro-wi-fi-am4-mini-itx-ddr4
[ram]: https://www.kabum.com.br/produto/103957/mem-ria-hyperx-fury-16gb-2666mhz-ddr4-cl16-preto-hx426c16fb3-16
[gpu]: https://www.kabum.com.br/produto/115393/placa-de-v-deo-sapphire-pulse-amd-radeon-rx-5700-xt-8gb-gddr6-be-11293-09-20g
[nvme]: https://www.kabum.com.br/produto/111081/ssd-gigabyte-256gb-m-2-pcie-nvme-leituras-1700mb-s-e-grava-es-1100mb-s-gp-gsm2ne3256gntd
[ssd]: https://www.kabum.com.br/produto/85196/ssd-kingston-a400-120gb-sata-leitura-500mb-s-grava-o-320mb-s-sa400s37-120g
[power]: https://www.kabum.com.br/produto/99506/fonte-evga-700w-80-plus-white-100-w1-0700-k
[wifi]: https://pt.aliexpress.com/item/4000631796433.html?spm=a2g0s.9042311.0.0.57c9b90aFhHRqd
[case]: https://www.kabum.com.br/produto/64705/gabinete-cougar-qbx-mini-tower-1-fan-108m020002-00

### Benchmarks

#### Cinebench

[technolli]: https://www.technolli.com/
[bios]: https://www.youtube.com/watch?v=bFDDc7hQJKg
[efi]: https://github.com/cirocfc/Ryzentosh/blob/master/files/EFI.zip
[clover]: https://github.com/cirocfc/Ryzentosh/blob/master/files/Clover.zip
