I added the the following function to the example-file after the declaration of the switch_ready-function:

```Ruby
class SwitchDisconnected < Trema::Controller

  def switch_disconnected(datapath_id)

    logger.info "Bye #{datapath_id.to_hex}"

  end

end
```

When the command "stop 0xabc" is issued in a second terminal, the virtual switch is stopped and the message "Bye 0xabc" appears.