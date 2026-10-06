# debug
Select Master Template Pattern:
  [1] Hand + Arm (Integrated)
  [2] Hand Only
  [3] Arm Only
  [0] Default (Use sim_config.json)

Enter number [Default=1]: 2

Command: python MuJoCoHand3DSimulator/run_simulator.py --pattern pattern_hand_only

Traceback (most recent call last):
  File "C:\hand\XanteIntegratedUpperController\MuJoCoHand3DSimulator\run_simulator.py", line 31, in <module>
    from core.simulator import Simulator
  File "C:\hand\XanteIntegratedUpperController\MuJoCoHand3DSimulator\core\simulator.py", line 15, in <module>
    import mujoco
  File "C:\Users\PMTP25-8\AppData\Local\Programs\Python\Python314\Lib\site-packages\mujoco\__init__.py", line 38, in <module>
    ctypes.WinDLL(os.path.join(os.path.dirname(__file__), 'mujoco.dll'))
    ~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\PMTP25-8\AppData\Local\Programs\Python\Python314\Lib\ctypes\__init__.py", line 433, in __init__
    self._handle = self._load_library(name, mode, handle, winmode)
                   ~~~~~~~~~~~~~~~~~~^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "C:\Users\PMTP25-8\AppData\Local\Programs\Python\Python314\Lib\ctypes\__init__.py", line 451, in _load_library
    return _LoadLibrary(self._name, winmode)
OSError: [WinError 1114] ダイナミック リンク ライブラリ (DLL) 初期化ルーチンの実行に失敗しました。

------------------------------------------------------------
  Simulator exited.
------------------------------------------------------------
