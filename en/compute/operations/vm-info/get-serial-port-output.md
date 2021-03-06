# Getting serial port output

You can get the information that the VM outputs to the serial port. This can be useful for troubleshooting.

---

**[!TAB Management console]**

1. Select the folder the VM belongs to.
1. Click on the **Yandex Compute Cloud** tile.
1. Click on the line with the VM you need.
1. Go to the **Serial port** tab.

**[!TAB CLI]**

[!INCLUDE [default-catalogue](../../../_includes/default-catalogue.md)]

1. View the description of the command to get serial port output:

    ```
    $ yc compute instance get-serial-port-output --help
    ```

1. Select a VM, for example, `first-instance`:

    [!INCLUDE [compute-instance-list](../../_includes_service/compute-instance-list.md)]

1. Get the output of the serial port. The serial port's output is usually long, so it should be written to a file:

    ```
    $ yc compute instance get-serial-port-output first-instance > output.txt
    ```

**[!TAB API]**

To get the serial port output, use the [getSerialPortOutput](../../api-ref/Instance/getSerialPortOutput.md) method of the [Instance](../../api-ref/Instance/index.md) resource.

---
