# FX505DT-hackintosh-tips

Hi there, this is a guide that is supposed to help you hackintosh Your Asus FX505DT (or/and maybe your FX505DU or FX505DY)
To begin, first we need to disable CSM (Compatibility support module), but how do we do that? There's no such option in the UEFI BIOS to disable it. Well, There is.
To disable it. we have to go the Security section, and enable Secure boot support. No, that doesn't enable Secure boot. To enable secure boot we need to update the keys in there, which we don't want to do because with secure boot enabled, we can't boot Opencore, And Opencore is required to boot macOS.
