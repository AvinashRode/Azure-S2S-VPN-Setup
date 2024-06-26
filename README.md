## Azure-S2S-VPN-Setup

To configure a Site-to-Site (S2S) VPN connection between your on-premises network and Azure, you'll need several components and steps:

![Alt Text](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/raw/main/S2S%20VPN.jpg)

1. **Azure Setup**:
   - **Virtual Network**: Create a virtual network (VNet) in the Azure portal.
   - **Subnets**: Define one or more subnets within the virtual network.
   - **VPN Gateway**: Configure and deploy a VPN gateway in the virtual network.
   - **Gateway Subnet**: Create a gateway subnet within your virtual network.
   - **Public IP Address**: Allocate a public IP address for the VPN gateway.
   - **Local Network Gateway**: Define a local network gateway in Azure to represent your on-premises network.
  
    Here is the rough costing for our setup [Costing for Azure-S2S-VPN-Setup](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/Costing%20for%20Azure-S2S-VPN-Setup.md)

2. **On-Premises Setup**: <img src="https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/Open%20VPN.png" alt="Alt Text" width="20" height="20">
   - **On-premises VPN**: Have a compatible VPN device or software running on your on-premises network.
   - **Public IP Address**: Ensure your on-premises network has a public IP address or is accessible via a public IP address for the VPN connection.

3. **Configure VPN Gateway in Azure**:
   - When configuring a VPN gateway in Azure, you'll need to choose between two VPN types: Policy-based or Route-based (also known as static-routing or dynamic-routing). The choice between the two depends on your specific network requirements and configurations:
  
      [Configure VPN Gateway in Azure](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/Configure%20VPN%20Gateway%20in%20Azure.md)

4. **Configure Local Network Gateway in Azure**:
   - Define a local network gateway in Azure to represent your on-premises network. This includes specifying the public IP address or address range of your on-premises VPN device.
     
      [Configure Local Network Gateway in Azure](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/Configure%20Local%20Network%20Gateway%20in%20Azure.md)

5. **VPN Device Configuration**:
   - Configure your on-premises VPN device to establish a connection with the Azure VPN gateway. This involves setting up the VPN tunnel, encryption settings, and authentication parameters.
  
     [VPN Device Configuration](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/VPN%20Device%20Configuration.md)
     
6. **Connectivity Testing**:
   - Once the configurations are complete, initiate the VPN connection from your on-premises VPN device to the Azure VPN gateway.
   - Verify connectivity by checking for successful tunnel establishment and testing communication between resources in Azure and your on-premises network.
  
      [Connectivity Testing](https://github.com/AvinashRode/Azure-S2S-VPN-Setup/blob/main/Connectivity%20Testing.md)

7. **Network Routing**:
   - Ensure that appropriate network routing is configured on both the on-premises network and Azure to direct traffic between the two networks through the VPN tunnel.

By following these steps and configuring the necessary components both in Azure and on-premises, you can establish a Site-to-Site VPN connection between your on-premises network and Azure.
