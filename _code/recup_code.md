---
step: 3
description: Retrieving the code
---

The simple method: download the zip file
----------------------------------

The source code can be downloaded directly as a zip file on [GitHub](https://github.com/prunkdump/GNUVario-TTGO-T5). Just click on **Clone or download** and **Download zip**.

![GitHub download zip]({{"/assets/code_img/code1.jpg" | absolute_url}})

Extract the zip to the location of your choice. This will create a ** Gnuvario-TTGO-T5-master ** directory.

![GitHub zip download]({{"/assets/code_img/code2.jpg" | absolute_url}})

The Arduino IDE installation normally created a **Arduino** directory in your personal folder. <BR> Make sure this folder is empty and copy the Sources \ Beta Code \ Gnuvario-E and Sources \ Beta folders Code \ libraries in the **Gnuvario-TTGO-T5-master** folder in the **Arduino** folder.

**IMPORTANT**: In this Arduino folder, there must be only the files / libraries of the Gnuvario-E project.

![GitHub zip download]({{"/assets/code_img/dossierRootArduino.jpg" | absolute_url}})

The advanced method: using Git
-----------------------------

You can also get the source code with [Git](https://git-scm.com/). This is a better approach because with Git, you can update the code while keeping your preferred settings.

So install Git and make sure the **Arduino** folder in your home directory is empty. With bash, go to the **Arduino** directory, clone the repository and create a branch for you.

{% highlight shell_session%}
~ $ cd Arduino
~ / Arduino $ git clone https://github.com/prunkdump/GNUVario-TTGO-T5.git.
~ / Arduino $ git checkout -b myversion
{% endhighlight%}

So, whenever you want to update the code, type the following commands from the **Arduino** directory. The first two lines save your changes. The next two lines download the changes from the main branch of GitHub. The last one applies the change to your version.

{% highlight shell_session%}
~ / Arduino $ git add -A
~ / Arduino $ git commit -m 'change'
~ / Arduino $ git checkout master
~ / Arduino $ git pull
~ / Arduino $ git checkout myversion
~ / Arduino $ git merge master
{% endhighlight%}