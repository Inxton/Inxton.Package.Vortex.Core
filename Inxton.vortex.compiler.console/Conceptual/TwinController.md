# TwinController

TwinController is the root object that represents the .net counterpart of the entire PLC program. It is the entry point to the PLC program variables. TwinController contains instances of all PRGs (Program objects) and GVLs (Global Variable Lists).

TwinController class is named [PlcName]TwinController.

TwinController exposes two special properties 'Online' and 'Shadow'. **Online** gives access only to online variables (direct access to PLC's values )and reduces the exposure of members that are not related to online access. **Shadow** gives access to shadow value holder with no direct access to PLC's values.


><strong style="color:orange">NOTE</strong>: 
<span style="color:orange">
PRG's symbols are not present on the communication layer if not attached to a running task or if not called in a POU that is called in some task of the PLC.
</span>

See also

- [TwinObjects](TwinObjects.md)
- [PrimitiveTwins](../../Inxton.Vortex.Connector/Conceptual/PrimitiveTwins.md)
- [Twin concepts](Twins.md)
