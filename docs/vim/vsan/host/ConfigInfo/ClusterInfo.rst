.. _str: https://docs.python.org/2/library/stdtypes.html

.. _vSphere API 5.5: ../../../../vim/version.rst#vimversionversion9

.. _vmodl.DynamicData: ../../../../vmodl/DynamicData.rst


vim.vsan.host.ConfigInfo.ClusterInfo
====================================
  Host-local VSAN cluster configuration. This data object is used both for specifying and retrieving cluster configuration for a host participating in the VSAN service.
:extends: vmodl.DynamicData_
:since: `vSphere API 5.5`_

Attributes:
    uuid (`str`_, optional):

       VSAN service cluster UUID, in the string form "nnnnnnnn-nnnn-nnnn-nnnn-nnnnnnnnnnnn", where n are hexadecimal digits. If provided while enabling the VSAN service, this value will be used for the service cluster UUID. If omitted when enabling the VSAN service, a suitable UUID will be generated by the platform. This is a read-only value while the VSAN service is enabled.
    nodeUuid (`str`_, optional):

       VSAN node UUID for this host. This is a read-only value which is populated upon enabling of the VSAN service.
