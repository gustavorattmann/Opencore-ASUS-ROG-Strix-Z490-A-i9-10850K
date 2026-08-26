# Opencore ASUS ROG Strix Z490-A Intel I9 10850K

## O que é Hackintosh?

É a preparação de um computador que não seja criado pela Apple para instalação do sistema operacional Mac.

## O que é Opencore?

É responsável por fazer a configuração que permitirá o Mac reconhecer os dispositivos do seu computador e fazer com que eles trabalhem da forma espereda.

**Nota:** Para configurar o Opencore é necessário esforço, tempo, dedicação e aprendizado, mas não é nada que seja de outro mundo.

É sempre importante consultar a documentação oficial ou procurar auxílio na internet, pois cada dispositivo tem sua própria configuração.

## Dica

Para automatização da criação de EFI, vale a pena conhecer o OpCore Simplify, que cria a EFI com base em seu Windows, detectando seu hardware... Se seu hardware possui algumas diferenças do meu, aconselho a criar sua EFI com base nessa ferramenta. Há vários tutoriais de como utilizá-la, depois é só fazer os ajustes finais.

Mantenha sempre um backup da útlima versão do Opencore que você criar ou alterar em um pen drive, para prevenção e manutenção, além de armazenar em nuvem, sempre que precisar recuperar.

Faça uma análise nas pastas de Kexts, ACPI e drivers e remova o que não for utilizar, depois faça um OC Clean Snapshot na configuração do OC para atualizar apenas com o que manteve. Esse passo também deve ser feito se adicionar algo novo.

Outro ajuste necessário é adicionar uma SMBIOS válida para permitir que algumas funcionalidades executem da forma correta como FaceTime e Mensagens.

**Nota¹:** Caso enfrente lentidão durante o boot utilizando algum SSD NVME da Samsung, faça a alteração do valor da propriedade "**SetApfsTrimTimeout**" de "**-1**" para "**0**" (No meu antigo PC o tempo de boot que era cerca de 1 minuto caiu para 15 segundos, mas o atual não precisei). Pelo que vi no último firmware e versões do Mac esse problema já foi resolvido.

**Nota²:** Para problema de áudio, basta seguir com o tutorial do **perez987**. Baixe a versão do Kernel Debug Kit igual ou mais próxima da versão do seu Mac.

## Versão do Opencore

1.0.7

## Minha Versão do Mac

Tahoe (26.6.2)

## Versão mínima compatível com Mac

Monterey (12.1)

## Meu Hardware

- Processador: Intel Core i9-10850K Deca-Core 3.6 Ghz
- Memória: 2x16Gb DDR4 Hiksemi Armor U10 3200mhz
- Placa-mãe: ASUS ROG Strix Z490-A Gaming
- Placa de vídeo: Gainward NVIDIA GeForce RTX™ 3080 Phantom
- Fonte: XPG Core Reactor II VE 850W
- Armazenamento: SSD NVME WD Green SN350 1TB (Windows)
- SSD NVME Samsung 970 EVO Plus 500Gb (Mac)
- SSD SATA SanDisk 240Gb 2,5" (VM)
- HD Western Digital 1Tb 3,5" (Backup)
- Water Cooler: Gigabyte Gaming 360
- Controlador de fan: Hub Controller Round5
- Gabinete: Lian Li Lancool 207 RX

## Programas essenciais

[Opencore Configurator](https://mackie100projects.altervista.org/download/occ/) - Para configuração dinâmica do arquivo de extensão plist (Hoje eu uso 100% o Propertree)

[Hackintool](https://github.com/benbaker76/Hackintool) - Ferramenta essencial para ajudar na configuração e também para fazer patches

[Kext Updater](https://update.kextupdater.de/kextupdater/Kext%20Updater.zip) - Responsável por baixar o Opencore e as kexts quando precisarem ser atualizados

[ProperTree](https://github.com/corpnewt/ProperTree) - Para configuração de texto do arquivo de extensão plist

[MaciASL](https://github.com/acidanthera/MaciASL) - Para auxiliar a criar os patches de SSDT

[IORegistery](https://github.com/khronokernel/IORegistryClone) - Obter informações de hardware no Mac em tempo real

[OpCore Simplify](https://github.com/lzhoang2801/OpCore-Simplify) - A melhor ferramenta para criar uma EFI pelo Windows de forma automática (Facilita cerca de 90% do processo)

[AppleHDA back in Tahoe](https://github.com/perez987/AppleHDA-back-on-macOS-26-Tahoe) - Tutorial para reativar o AppleHDA no Mac Tahoe

[Apple Developer - Download](https://developer.apple.com/download/all/) - Baixar o KDK (Kernel Debug Kit) para execução do tutorial para reativação do AppleHDA. A versão deve ser igual ou mais próxima possível da versão do seu Mac.

## Links de auxílio

[Documentação oficial](https://dortania.github.io/OpenCore-Install-Guide/)

[Grupo Hackintosh Brasil - Facebook](https://www.facebook.com/groups/hackintoshbrazil)

[Canal do Gabriel Luchina](https://www.youtube.com/@UniversoHackintosh)

[Canal do Dicas do Mateus](https://www.youtube.com/@DicasdoMateus)
