# Android Bluetooth Printer
Android library for using thermal printers via bluetooth connection.

## Example usage
```
BluetoothAdapter btAdapter = BluetoothAdapter.getDefaultAdapter();
BluetoothDevice mBtDevice = btAdapter.getBondedDevices().iterator().next();   // Get first paired device

final BluetoothPrinter mPrinter = new BluetoothPrinter(mBtDevice);
mPrinter.connectPrinter(new BluetoothPrinter.PrinterConnectListener() {
  
  @Override
  public void onConnected() {
    
  }
  
  @Overide
  public void onFailed() {
  
  }
  
});

```
