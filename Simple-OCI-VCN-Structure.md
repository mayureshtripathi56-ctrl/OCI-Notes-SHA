# Create a Simple OCI VCN Structure in draw.io

This lab creates a basic OCI VCN diagram containing only:

- OCI Region
- Virtual Cloud Network (VCN)
- Public Subnet
- Private Subnet

The following example values are used:

| Component | Name / CIDR |
|---|---|
| Region | India South (Hyderabad) |
| VCN | `sha-learning-vcn` |
| VCN CIDR | `10.0.0.0/16` |
| Public Subnet | `10.0.1.0/24` |
| Private Subnet | `10.0.2.0/24` |

## Step 1: Open draw.io

1. Open [https://app.diagrams.net/](https://app.diagrams.net/).
2. Select **Device** if draw.io asks where the diagram should be stored.
3. Click **Create New Diagram**.
4. Select **Blank Diagram**.
5. Enter a diagram name and click **Create**.

The blank editor opens with the shape panel on the left, drawing canvas in the centre, and formatting panel on the right.

![Step 1 - Open a blank draw.io diagram](assets/oci-vcn-simple-01-open-blank-editor.jpg)

## Step 2: Create the OCI Region Boundary

1. From the **General** shapes section, drag a **Rectangle** or **Vertical Container** onto the canvas.
2. Resize it so that it forms the outer boundary of the diagram.
3. Double-click the heading and enter:

   `OCI Region: India South (Hyderabad)`

4. In the **Style** panel:
   - Set the border colour to OCI red.
   - Use a very light red fill.
   - Enable rounded corners if required.
5. Add a text box above the boundary with the title:

   `Simple OCI VCN Structure — Public and Private Subnets`

![Step 2 - Create the OCI Region boundary](assets/oci-vcn-simple-02-create-region-boundary.jpg)

## Step 3: Create the VCN Boundary

1. Drag another large rectangle inside the Region boundary.
2. Leave space on all sides so the VCN is clearly shown as part of the Region.
3. Double-click the heading and enter:

   `VCN: sha-learning-vcn | CIDR: 10.0.0.0/16`

4. In the **Style** panel:
   - Set the fill colour to white.
   - Set the border colour to dark grey.
   - Select a dashed border style.

The hierarchy should now be:

`OCI Region → VCN`

![Step 3 - Add the VCN boundary](assets/oci-vcn-simple-03-add-vcn-boundary.jpg)

## Step 4: Add the Public Subnet

1. Drag a smaller horizontal container inside the upper half of the VCN.
2. Double-click its heading and enter:

   `PUBLIC SUBNET | 10.0.1.0/24`

3. In the **Style** panel:
   - Set the border colour to green.
   - Use a light green fill for the heading area.
   - Keep the main subnet area white or very light green.
4. Resize the container so there is enough empty space for future public resources.

![Step 4 - Add the public subnet](assets/oci-vcn-simple-04-add-public-subnet.jpg)

## Step 5: Add the Private Subnet

1. Copy and paste the Public Subnet container, or drag another horizontal container into the lower half of the VCN.
2. Double-click its heading and enter:

   `PRIVATE SUBNET | 10.0.2.0/24`

3. Change its formatting:
   - Set the border colour to blue.
   - Use a light blue fill for the heading area.
   - Keep the main subnet area white or very light blue.
4. Select both subnet containers.
5. Use **Arrange → Align → Center** so that both containers have the same horizontal alignment.
6. Resize them to the same width.

The completed structure should now be:

`OCI Region → VCN → Public Subnet + Private Subnet`

![Step 5 - Add the private subnet and complete the structure](assets/oci-vcn-simple-05-add-private-subnet-final.jpg)

## Step 6: Save the Editable draw.io File

1. Click the diagram name in the upper-left corner and rename it:

   `OCI_VCN_Reference_Structure.drawio`

2. Select **File → Save As**.
3. Keep **XML File (.drawio)** as the file type.
4. Select **Download** or **Device** as the location.
5. Click **OK**.

The `.drawio` file can be reopened later to edit individual containers, labels, colours, and CIDR blocks.

![Step 6 - Save the editable draw.io file](assets/oci-vcn-simple-06-save-drawio-file.jpg)

## Step 7: Open the PNG Export Option

1. Select **File** from the top menu.
2. Point to **Export as**.
3. Select **PNG**.

![Step 7 - Select File, Export as, PNG](assets/oci-vcn-simple-07-export-png-menu.jpg)

## Step 8: Export a High-Resolution PNG

1. Set **Zoom** to `150%` for clearer text in the wiki.
2. Keep **Size** set to **Diagram**.
3. Leave **Transparent Background** unchecked so the image has a white background.
4. Keep **Include a copy of my diagram** checked. This embeds the diagram data in the PNG so it can be reopened in draw.io.
5. Click **Export**.
6. Enter the file name:

   `OCI_VCN_Reference_Structure_Wiki_Final.png`

7. Select **Download** and click **OK**.

![Step 8 - Configure the PNG export](assets/oci-vcn-simple-08-export-settings.jpg)

## Final Diagram

![Simple OCI VCN structure with public and private subnets](assets/OCI_VCN_Reference_Structure_Wiki_Final.png)

## CIDR Check

- The VCN uses `10.0.0.0/16`.
- The Public Subnet uses `10.0.1.0/24`.
- The Private Subnet uses `10.0.2.0/24`.
- Both subnet CIDR blocks are contained within the VCN CIDR block.
- The two subnet CIDR blocks do not overlap.

## References

- [draw.io online editor](https://app.diagrams.net/)
- [Save diagram files in draw.io](https://www.drawio.com/docs/getting-started/save-diagram-files/)
- [Export a draw.io diagram to PNG](https://www.drawio.com/docs/manual/export/export-to-png/)
- [OCI Networking Overview](https://docs.oracle.com/en-us/iaas/Content/Network/Concepts/overview.htm)
