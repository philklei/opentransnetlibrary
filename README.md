Opentrans .NET Library
===================

Welcome to .NET openTrans Libary.

This libary supports to serialize or deserialize Opentrans Documents an parse them into our classes. with this libary you can simply create and read xml documents. Each class in this libary has implemented an serialize, deserialize, save to file and load from file function.

The example shows how simply this class works:


Dim order As New Opentrans.ORDER

order.version = Opentrans.typeOPENTRANS_version.Item21
order.type = Opentrans.ORDERType.standard

order.ORDER_HEADER.CONTROL_INFO.GENERATION_DATE = Now.ToLongTimeString
order.ORDER_HEADER.CONTROL_INFO.GENERATOR_INFO = "COMPANY SERVICE GENERATOR"

....

Dim orderXML as string = order.Serialize()


You can download a 30 days trail version of this Libary from: Opentrans.rar

If you a interested to get a full version of this libary you can contact me via email: philip.kleimeyer@gmail.com
