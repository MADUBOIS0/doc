---
eleventyComputed:
  title: Duplicate {{ en.DVLS }} Instance
---
When you open the {{ en.DVLSCONSOLE }}, two instances of the same {{ en.DVLS }} are visible in the {{ en.DVLSCONSOLE }}. One with only a "/" as the Web Application Name.
![!!KB4298](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4298.png)

## Cause 1

Using the default parameters of the IIS Manager, the Default Web Site points to the same Physical Path of the {{ en.DVLS }} web application.

### Steps

Change the path of the Web Site in the IIS Manager.

1. Open IIS Manager, select the ***Web Site*** that contains the {{ en.DVLS }} web application and click on ***Advanced Settings*** in the ***Actions*** panel on the right.
![!!KB4299](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4299.png)
1. Change the ***Physical Path*** of the Web Site from the {{ en.DVLS }} subfolder to the parent folder.
![!!KB4300](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4300.png)
![!!KB4301](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4301.png)
1. **Restart your IIS Server**.
![!!KB4302](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4302.png)
1. On the {{ en.DVLSCONSOLE }}, click on the ***Refresh*** button and just one instance should be displayed.
![!!KB4303](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4303.png)

## Cause 2
When the Web Site is located in a different folder then the default one used by the IIS Manager, the Web Site points to the same Physical Path of the {{ en.DVLS }} web application.
![!!KB4304](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4304.png)

### Steps

To have only one {{ en.DVLS }} instance without any duplicate, the Physical path of the instance must be points to a subfolder of the Web Site Physical Path.

1. **Open the Windows Explorer** and create a folder in the ***Physical Path*** of the Web Site. In the image below, the name of the new folder is {{ en.DVLS }} It can be another folder name that fits your needs.
![!!KB4305](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4305.png)
1. Move the selected files and folders into that new subfolder, i.e. {{ en.DVLS }}.
![!!KB4306](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4306.png)
1. Open the IIS Manager and select the {{ en.DVLS }} web application in the Tree View and click on ***Advanced Settings*** in the ***Action*** panel on the right.
![!!KB4307](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4307.png)
1. Change the ***Physical Path*** to point to the new folder created in step 1.
![!!KB4308](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4308.png)
1. To restart your IIS Server, select the root in the **Tree View** and click on ***Restart*** in the ***Actions*** panel on the right.
![!!KB4309](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4309.png)
1. On the {{ en.DVLSCONSOLE }}, click on the ***Refresh*** button and just one instance should be displayed.
![!!KB4310](https://cdnweb.devolutions.net/docs/docs_en_kb_KB4310.png)
