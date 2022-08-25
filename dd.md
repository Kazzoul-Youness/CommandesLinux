LINUX : DD

COPIE :

	* devices

	* partitions ou volume logique

	* disque ou zones de disque

	* local ou distant (combinaison avec ssh)



-----------------------------------------
LINUX : DD


copie de disk à disk

```
dd if=/dev/sdb of=/dev/sdc
dd if=/dev/sdb of=/dev/sdc status=progress
```


-----------------------------------------
LINUX : DD


copie en format image (copie sur cd ou usb)

```
dd if=/dev/sdb of=myimage.img
```


-----------------------------------------
LINUX : DD


restauration

```
dd if=myimage.img of=/dev/sdc
```


-----------------------------------------
LINUX : DD


nettoyer

```
dd if=/dev/zero of=/dev/sdc
dd if=/dev/random of=/dev/sdc
```
