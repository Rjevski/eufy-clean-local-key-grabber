# Eufy device ID & key grabber

This Python program allows you to obtain the device ID & local key for your Eufy devices without having to rely on running an old version of their Android app.

## **UNMAINTAINED**

I am not sure if this is still working (there's a massive security vulnerability with how the client authenticated to Tuya, so there's a chance they've now fixed it and as a result this tool will need updating); I do not currently use it anymore and have little time to maintain it. I'd be happy to appoint a maintainer if someone volunteers.

## Usage/TLDR:

In a somewhat recent Python 3 (I ran Python 3.9 when developing this) virtualenv, run the following:

```shell
pip install -r requirements.txt
python -m eufy_local_id_grabber "<EUFY ACCOUNT EMAIL>" "<EUFY ACCOUNT PASSWORD>"
```

You will get the following output:

```
Home: <home ID>
Device: RoboVac, device ID <device ID>, local key <local key>
```

It will list all the devices in all the "homes" (though I am actually not sure if you can have more than one home in Eufy) on your account.

## Credits & Thanks

* https://github.com/mitchellrj/eufy_robovac
* https://github.com/nalajcie/tuya-sign-hacking
* https://github.com/TuyaAPI/cloud

And the other amazing people who've shown interest in this project and even contributed to it. ❤️
