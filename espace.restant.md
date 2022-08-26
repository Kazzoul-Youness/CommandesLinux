Les fichiers qui ont une taille moins 100 octet, et qui se trouve là ou vous lancer la commande

du -s * | sort -n | awk '{if ($1 < 100) print $1,"octet" ," --> ",$2}'
