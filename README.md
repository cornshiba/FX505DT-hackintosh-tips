# FX505DT-hackintosh-tips

Note: I am **NOT** responsible for any damage you do to your laptop using these tips. Continue at your own risk.

Hi there, this is a guide that is supposed to help you hackintosh Your Asus FX505DT (or/and maybe your FX505DU or FX505DY)

# Disabling CSM
To begin, first we need to disable CSM (Compatibility support module), but how do we do that? There's no such option in the UEFI BIOS to disable it. Well, There is. To disable it. we have to go the Security section, and enable Secure boot support. No, that doesn't enable Secure boot. To enable secure boot we need to update the keys in there, which we don't want to do because with secure boot enabled, we can't boot Opencore, And Opencore is required to boot macOS.

It should look like this if you did it right:
![CSM](CSMdisable.gif)

# Enabling Above 4G Decoding
Great, we disabled CSM, now we need to enable Above 4g decoding so we have to use ncpi=0x2000. To begin, first we need to download Smokeless-UMAF, this is a tool that is used to change hidden settings in the UEFI BIOS; And No, it is not modifying the UEFI BIOS directly. Oh, and we need to be really careful with this tool, because you can brick your laptop if something is done wrong using this tool! Alright, back to the UMAF stuff. You need to download it, follow the tutorial on how to install it, and after that, boot up this tool. Great! Now we're in smokeless-UMAF. First we need to go to Device manager --> then check if you PCI Subsystem settings, if you do --> open it --> Select Above 4g decoding and enable it. to save configuration changes, press F10. now we need to restart in order to apply these settings. Great! we enabled Above 4g decoding.

Here's where its located:
![Above4GDecoding](Above4GDecoding.gif)
To enable the first option, just click enter. to save it click F10.
