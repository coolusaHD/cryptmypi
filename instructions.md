# Configurations

```shell
## USB KEY PATH - ADD TRAILING SLASH
export _USBKEYPATH="/media/whatever/9ecfba84-47d4-4495-a7db-418fdce15cad/"

## KEY FILE NAME
#
#  To gen a valid key use:
#    sudo dd bs=32 count=1 if=/dev/random of=dec.key
#
export _KEYFILENAME="dec.key"

## USB UUID
export _USBUUID="9ecfba84-47d4-4495-a7db-418fdce15cad"
```

# Extra Hooks

## Unlock Script
`3000-stage1-setup-encryption.hook:66` 

## Add USB Key as a Trusted Key for LUKS decryption
`5200-stage2-setup-luks-create.hook:40`