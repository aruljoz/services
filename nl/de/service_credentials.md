---

copyright:

  years: 2015, 2017
lastupdated: "2017-08-01"

---

{:new_window: target="_blank"}  
{:shortdesc: .shortdesc}


# Neuen Serviceberechtigungsnachweis hinzufügen
{: #service_credentials}

Sie können eine neue Gruppe von Serviceberechtigungsnachweisen für die Fälle generieren, in denen Sie einen externen Konsumenten manuell mit einem Bluemix-Service verbinden möchten. Wenn Sie beispielsweise versuchen, eine AWS-App an einen Watson-Service zu binden, müssen Sie einen neuen Serviceberechtigungsnachweis generieren, der für die Bindung dieser beiden Services verwendet werden kann.

Cloud Foundry-Services können einen Serviceschlüssel - auch als Serviceberechtigungsnachweis bezeichnet - generieren. Serviceberechtigungsnachweise sind servicespezifisch und variieren abhängig davon, wie der jeweilige Service die Berechtigungsnachweise definiert, die generiert werden müssen. Ein Serviceberechtigungsnachweis kann zum Beispiel einen Benutzernamen, ein Kennwort, einen Hostnamen, einen Port und eine URL enthalten. Der Inhalt des jeweiligen Serviceberechtigungsnachweises ist jedoch für den Service, der ihn generiert, eindeutig. Einige Services generieren möglicherweise zusätzliche Daten, für die die Angabe von Parametern erforderlich ist. So kann es bei einem Service zum Beispiel erforderlich sein, einen Sprachparameter einzugeben, mit dem die Standardsprache festgelegt wird, die im generierten Serviceschlüssel zurückgegeben wird. 

Führen Sie die folgenden Schritte aus, um einen neuen Serviceberechtigungsnachweis hinzuzufügen:

1. Wählen Sie auf der Servicedetailseite die Registerkarte mit den Serviceberechtigungsnachweisen aus und klicken Sie auf **Neuen Berechtigungsnachweis + **.
2. Geben Sie im Dialogfeld für das Hinzufügen eines neuen Berechtigungsnachweises einen **Name** an.
3. Optional können Sie zusätzliche Parameter als gültiges JSON-Objekt mit servicespezifischen Konfigurationsparametern inline oder in einer Datei angeben.

  **Hinweis**. Für die meisten Services sind keine zusätzlichen Parameter erforderlich. Bei den Services, die zusätzliche Parameter erfordern, definiert jeder Service eine eigene Parameterliste. Eine Liste der unterstützten Konfigurationsparameter finden Sie in der Dokumentation für das jeweilige Serviceangebot.
4. Klicken Sie auf **Hinzufügen**, um den neuen Serviceberechtigungsnachweis zu generieren.
