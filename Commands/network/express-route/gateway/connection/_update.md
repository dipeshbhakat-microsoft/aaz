# [Command] _network express-route gateway connection update_

Update an ExpressRoute gateway connection.

## Versions

### [2022-01-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL2V4cHJlc3Nyb3V0ZWdhdGV3YXlzL3t9L2V4cHJlc3Nyb3V0ZWNvbm5lY3Rpb25zL3t9/2022-01-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/expressroutegateways/{}/expressrouteconnections/{} 2022-01-01 -->

#### examples

- Update an ExpressRoute gateway connection.
    ```bash
        network express-route gateway connection update --gateway-name MyGateway -n MyExpressRouteConnection -g MyResourceGroup --peering /subscriptions/MySub/resourceGroups/MyResourceGroup/providers/Microsoft.Network/expressRouteCircuits/MyCircuit/peerings/AzurePrivatePeering --associated-route-table /MySub/resourceGroups/MyResourceGroup/providers/Microsoft.Network/virtualHubs/MyHub/hubRouteTables/MyRouteTable1 --propagated-route-tables [/MySub/resourceGroups/MyResourceGroup/providers/Microsoft.Network/virtualHubs/MyHub/hubRouteTables/MyRouteTable1,/MySub/resourceGroups/MyResourceGroup/providers/Microsoft.Network/virtualHubs/MyHub/hubRouteTables/MyRouteTable2] --labels [label1,label2]
    ```