
hfsts 1
cmd> -> Getting status for FINGER_1...

--- FINGER_1 Status ---
  MP Angle                  : -0.00
  PIP/DIP Angle             : -0.06

Shutting down controller...
Network command listener stopped.
Releasing shared memory pointers...
Traceback (most recent call last):
  File "c:\hand\XanteIntegratedUpperController\hand_controller\system_controller.py", line 310, in main
    _dispatch_user_command(command_line, shm_mgr, context)
  File "c:\hand\XanteIntegratedUpperController\hand_controller\system_controller.py", line 195, in _dispatch_user_command
    command_map[command](args, shm_mgr, context)
  File "c:\hand\XanteIntegratedUpperController\hand_controller\hand_lib\handlers\hand_xante_command_handlers.py", line 174, in handle_finger_status
    print(f"  AbAd Angle                : {abad:.2f}")
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
TypeError: unsupported format string passed to NoneType.__format__

During handling of the above exception, another exception occurred:

Traceback (most recent call last):
  File "c:\hand\XanteIntegratedUpperController\hand_controller\system_controller.py", line 407, in <module>
    main()
  File "c:\hand\XanteIntegratedUpperController\hand_controller\system_controller.py", line 375, in main
    miniarm_command_handler.handle_ma_disconnect([], shm_mgr, context)
                                                              ^^^^^^^
UnboundLocalError: cannot access local variable 'context' where it is not associated with a value
Exception ignored in: <function SharedMemory.__del__ at 0x00000213A8611800>
Traceback (most recent call last):
  File "C:\Users\PMTP25-8\AppData\Local\Programs\Python\Python311\Lib\multiprocessing\shared_memory.py", line 187, in __del__
    self.close()
  File "C:\Users\PMTP25-8\AppData\Local\Programs\Python\Python311\Lib\multiprocessing\shared_memory.py", line 230, in close
    self._mmap.close()
BufferError: cannot close exported pointers exist
PS C:\hand\XanteIntegratedUpperController> 
