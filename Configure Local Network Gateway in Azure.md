## Configure Local Network Gateway in Azure

To configure a Local Network Gateway (LNG) in Azure, representing your on-premises network, follow these steps:

1. **Sign in to the Azure Portal**:
   - Navigate to the Azure portal at https://portal.azure.com.
   - Sign in with your Azure account credentials.

2. **Create a Local Network Gateway**:
   - In the Azure portal, click on "Create a resource" in the upper left corner.
   - In the search box, type "Local Network Gateway" and press Enter.
   - Select "Local Network Gateway" from the search results, then click "Create" to begin the creation process.

3. **Configure the Local Network Gateway**:
   - In the "Basics" tab of the creation wizard:
     - Enter a name for your local network gateway.
     - Choose the subscription and resource group where you want to create the local network gateway.
     - Select the region where the local network gateway will be located.
   - Click "Next: IP Addresses" to proceed.

4. **Specify IP Addresses**:
   - In the "IP Addresses" tab:
     - Enter the public IP address or address range of your on-premises VPN device.
     - Optionally, you can also specify multiple IP address ranges if your on-premises network spans multiple subnets.
   - Click "Review + create" to proceed.

5. **Review and Create**:
   - Review the configuration settings to ensure they are correct.
   - Click "Create" to create the local network gateway.

6. **Wait for Deployment**:
   - Azure will begin deploying the local network gateway. Wait for the deployment to complete, which may take a few minutes.

7. **Verification**:
   - Once the deployment is complete, navigate to the Local Network Gateway resource in the Azure portal.
   - Verify that the settings match the configuration of your on-premises network, including the specified public IP address or address range.

