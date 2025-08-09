> Achtung: Das Projekt wird nicht mehr gepflegt
>
> Da das Projekt schon lange besteht und die verwendete Technologie veraltet ist und ich keine Energie mehr für die Aktualisierung dieses Projekts habe, habe ich beschlossen, das Projekt zu archivieren. Sie können stattdessen andere Projekte verwenden.
>
> Wenn Sie dieses Projekt weiterhin verwenden müssen, ist die beste Möglichkeit, Version 2.94 in Docker zu verwenden und eine Umgebungsvariable für die WebUI festzulegen. Siehe dazu ([https://www.cnblogs.com/ronggang/p/18788723](https://www.cnblogs.com/ronggang/p/18788723)); oder verwenden Sie andere bereits integrierte Projekte.
>
> Vielen Dank für Ihre langjährige Unterstützung.
>
> 01.06.2025 Zaipeizhe (der Kultivierende)

-----

\<p align="center"\>
\<img src="[https://github.com/ronggang/transmission-web-control/raw/master/src/tr-web-control/logo.png](https://github.com/ronggang/transmission-web-control/raw/master/src/tr-web-control/logo.png)"\>\<br/\>
\<a href="[https://github.com/ronggang/transmission-web-control/releases](https://github.com/ronggang/transmission-web-control/releases)" title="GitHub Releases"\>\<img src="[https://img.shields.io/github/release/ronggang/transmission-web-control.svg](https://img.shields.io/github/release/ronggang/transmission-web-control.svg)"\>\</a\>
\<img src="[https://img.shields.io/badge/transmission-%3E=2.40%20(RPC%20%3E14)-green.svg](https://img.shields.io/badge/transmission-%3E=2.40%20\(RPC%20%3E14\)-green.svg)" title="Unterstützte Transmission Version"\>
\<a href="[https://github.com/ronggang/transmission-web-control/LICENSE](https://github.com/ronggang/transmission-web-control/LICENSE)" title="GitHub Lizenz"\>\<img src="[https://img.shields.io/github/license/ronggang/transmission-web-control.svg](https://img.shields.io/github/license/ronggang/transmission-web-control.svg)"\>\</a\>
\<a href="[https://t.me/transmission\_web\_control](https://t.me/transmission_web_control)"\>\<img src="[https://img.shields.io/badge/Telegram-Chat-blue.svg?logo=telegram](https://img.shields.io/badge/Telegram-Chat-blue.svg?logo=telegram)" alt="Telegram"/\>\</a\>
\</p\>

-----

## [English Introduction](https://github.com/ronggang/transmission-web-control/wiki)

## Inländische Mirror-Quelle

  - https://gitee.com/culturist/transmission-web-control

## Über

Das Hauptziel dieses Projekts ist es, die Bedienbarkeit der [Transmission](https://www.transmissionbt.com/) Web-Oberfläche zu verbessern. Dieses Projekt wurde ursprünglich auf [Google Code](https://code.google.com/p/transmission-control/) gehostet und wurde nun zu GitHub migriert.
Dieses Projekt wurde ursprünglich für PT-Seiten (Private Tracker) entworfen, weshalb es eine Gruppierung und Statusanzeige für Tracker-Server hinzufügt, was für normale BT-Torrents nicht geeignet ist.

Darüber hinaus ist dieses Projekt nur eine benutzerdefinierte WebUI und kann Transmission nicht ersetzen. Benutzer müssen Transmission selbst installieren, damit es ordnungsgemäß funktioniert. Anweisungen zur Installation von Transmission finden Sie auf der offiziellen Website: [https://www.transmissionbt.com/](https://www.transmissionbt.com/)

## Benutzeroberfläche-Vorschau

## Installationsanweisungen und weitere Inhalte finden Sie hier: [Chinesische Hilfe](https://github.com/ronggang/transmission-web-control/wiki/Home-CN)

### DSM7.0

In dieser Version müssen zusätzliche Berechtigungen geändert werden, um die automatische Aktualisierungsfunktion zu ermöglichen.
Führen Sie die folgenden Befehle mit `root`-Rechten aus, wobei:

  - `YOUR_USERNAME` durch den Benutzernamen ersetzt wird, den Sie für die Anmeldung und das Ausführen des Update-Skripts verwenden.
  - `/var/packages/transmission/target/share/transmission/web/` der Installationspfad von Transmission ist (standardmäßig sollte es dieser sein).

<!-- end list -->

```shell
sed -i '/sc-transmission/s/$/YOUR_USERNAME/' /etc/group
chown sc-transmission:sc-transmission /var/packages/transmission/target/share/transmission/web/* -R
chmod 774 /var/packages/transmission/target/share/transmission/web/* -R
```

## Änderungslog [Anzeigen](https://github.com/ronggang/transmission-web-control/blob/master/CHANGELOG.md)

## Tägliche Projektpflege

  * Zaipeizhe (der Kultivierende)
  * DarkAlexWang
