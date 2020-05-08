# seafile-Blue-Dark-Theme
For the cloud software <strong>seafile</strong> a custom theme in Dark Blue ;-)

<h2>Usage / Installation</h2>
Switch to user <code>seafile</code> and create the folder <strong>custom</strong> and folder <strong>img</strong>:
<br><br>
<pre>
<code>sudo su seafile</code>
<code>cd</code>
<code>mkdir /home/seafile/sea-hub/custom</code>
<code>mkdir /home/seafile/seahub-data/img</code>
</pre>

<h2>Create Symlinks</h2>
ln -s /home/seafile/seahub-data/custom /home/seafile/seafile-server-latest/seahub/media/custom
<br>
ln -s /home/seafile/seahub-data/img /home/seafile/seafile-server-latest/seahub/media/images
<br><br>
<h2>Procedure</h2>
Copy the entire contents of the <code>custom</code> and <code>img</code> folder to the <strong>seahub-data/custom</strong> and <strong>seahub-data/img</strong>. The Owner of these folders and files must be seafile.
<br><br>
Edit the File: <strong>conf/seahub_settings.py</strong>

<pre>
<code>BRANDING_CSS = 'custom/custom.css'</code>
<code>FILE_SERVER_ROOT = 'https://your_ip_adresse_or_dyndns.com/seafhttp'</code>
<code>FAVICON_PATH = 'custom/favicon.png'</code>
<code>LOGO_PATH = 'custom/custom-logo.png'</code>
<code>LOGO_WIDTH = 160</code>
<code>LOGO_HEIGHT = 40</code>
</pre>

Optionally you can use the logo/favicon or login background or your own picture. Alternatively, you can use the folder file <code>folder-192.png</code> and copy from /img to:
<pre><code>/home/seafile/seafile-server-latest/seahub/media/img/</code></pre>

Then the Seafile server and Seahub must be restarted.
<pre>
<code>sudo systemctl restart seafile.service</code>
<code>sudo systemctl restart seahub.service</code>
</pre>

Have Fun ;-)

<h2>Screenshots</h2>
<img src="https://github.com/topa-LE/seafile_blue_dark_themes/blob/master/Screenshots/screen-2.png?raw=true" alt="Folder" style="max-width:100%;" width="400">

<img src="https://github.com/topa-LE/seafile_blue_dark_themes/blob/master/Screenshots/screen-4.png?raw=true" alt="Folder" style="max-width:100%;" width="400">

<img src="https://github.com/topa-LE/seafile_blue_dark_themes/blob/master/Screenshots/screen-6.png?raw=true" alt="Folder" style="max-width:100%;" width="400">

<pre>You can find more screens in the folder: <a href="https://github.com/topa-LE/seafile-Blue-Dark-Theme/tree/master/Screenshots">Screenshots</a></pre>
