##��������� ������:

| type |  Flag  | UUID 02  | UUID 16   | UUID 16 Data                       |
| ---- | ------ | -------- | --------- | ---------------------------------- |
| msg  | 020106 | 030250fd | 141650fd  | 488040000001b36eb30d64e80a4d9cbc38 |
| adv  | 020106 | 030250fd | 141650fd  | 490000080c9c105bc01d9f87           |

adv - ���������� ������.

msg - ���������� ��� ��������� ����������� �/��� ���������.

##Adv ��������:

�� bond - pid ����������, ����� bond - ������������� device_id � login_key � device_id

##����� ������, ����� ����������� ���������������, ����������� ���:

[7] pid_len+7

[11,12] Frame Control:
bound_flag |0x08, DEVICE_SHARED |0x04, connect request bit |0x02

[13] pid_type

[14] pid_len

[15...] code

��������� https://github.com/tuya/tuya-ble-sdk/blob/main/sdk/src/tuya_ble_main.c#L453