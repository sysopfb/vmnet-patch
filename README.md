# vmnet-patch
vmnet patch for vmware workstation on 3.18


to install

cd /usr/lib/vmware/modules/source
tar -xvf vmnet.tar
patch vmnet-only/netif.c < ~/path/to/netif-patch.patch
tar -uvf vmnet.tar vmnet-only
rm -r vmnet-only
