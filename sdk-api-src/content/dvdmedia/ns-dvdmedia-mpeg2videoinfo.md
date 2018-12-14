---
UID: NS:dvdmedia.tagMPEG2VIDEOINFO
title: MPEG2VIDEOINFO
author: windows-sdk-content
description: The MPEG2VIDEOINFO structure describes an MPEG-2 video stream.
old-location: dshow\mpeg2videoinfo.htm
tech.root: DirectShow
ms.assetid: 1a6ab686-99a1-40c2-addf-7fa215e2311a
ms.author: windowssdkdev
ms.date: 12/5/2018
ms.keywords: AMMPEG2_27MhzTimebase, AMMPEG2_DSS_UserData, AMMPEG2_DVB_UserData, AMMPEG2_DVDLine21Field1, AMMPEG2_DVDLine21Field2, AMMPEG2_DoPanScan, AMMPEG2_FilmCameraMode, AMMPEG2_LetterboxAnalogOut, AMMPEG2_SourceIsLetterboxed, AMMPEG2_WidescreenAnalogOut, MPEG2VIDEOINFO, MPEG2VIDEOINFO structure [DirectShow], MPEG2VIDEOINFOStructure, dshow.mpeg2videoinfo, dvdmedia/MPEG2VIDEOINFO, tagMPEG2VIDEOINFO
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: dvdmedia.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Dvdmedia.h
api_name:
 - MPEG2VIDEOINFO
product: Windows
targetos: Windows
req.typenames: MPEG2VIDEOINFO
req.redist: 
---

# MPEG2VIDEOINFO structure


## -description


The <b>MPEG2VIDEOINFO</b> structure describes an MPEG-2 video stream.
        


## -struct-fields




### -field hdr


<a href="https://msdn.microsoft.com/en-us/library/Dd407326(v=VS.85).aspx">VIDEOINFOHEADER2</a> structure.
          


### -field dwStartTimeCode

25-bit group-of-pictures (GOP) time code at start of data. This field is not used for DVD.
          


### -field cbSequenceHeader

Length of the sequence header, in bytes. For DVD, set this field to zero. The sequence header is given in the <b>dwSequenceHeader</b> field.
          


### -field dwProfile

Specifies the MPEG-2 profile as an <a href="https://msdn.microsoft.com/en-us/library/Dd373479(v=VS.85).aspx">AM_MPEG2Profile</a> enumeration type.
          


### -field dwLevel

Specifies the MPEG-2 level as an <a href="https://msdn.microsoft.com/en-us/library/Dd373478(v=VS.85).aspx">AM_MPEG2Level</a> enumeration type.
          


### -field dwFlags

Flag indicating preferences. Set one or a combination of the following values.
          

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_DoPanScan"></a><a id="ammpeg2_dopanscan"></a><a id="AMMPEG2_DOPANSCAN"></a><dl>
<dt><b>AMMPEG2_DoPanScan</b></dt>
<dt>0x00000001</dt>
</dl>
</td>
<td width="60%">
If this flag is set, the MPEG-2 video decoder should crop the output image based on pan-scan vectors in picture_display_extension and change the picture aspect ratio to 4x3. The VMR should not receive a 16x9 sample with this flag. A simple implementation might alter the source rectangle to indicate a 540 wide source region with a left edge equal to the display offset in the picture_display_extension.

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_DVDLine21Field1"></a><a id="ammpeg2_dvdline21field1"></a><a id="AMMPEG2_DVDLINE21FIELD1"></a><dl>
<dt><b>AMMPEG2_DVDLine21Field1</b></dt>
<dt>0x00000002</dt>
</dl>
</td>
<td width="60%">
If set, the MPEG-2 decoder must be able to produce an output pin for DVD style closed-captioned data found in the Group Of Pictures (GOP) layer of field 1. 

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_DVDLine21Field2"></a><a id="ammpeg2_dvdline21field2"></a><a id="AMMPEG2_DVDLINE21FIELD2"></a><dl>
<dt><b>AMMPEG2_DVDLine21Field2</b></dt>
<dt>0x00000004</dt>
</dl>
</td>
<td width="60%">
If set, the MPEG-2 decoder must be able to produce an output pin for DVD style closed-captioned data found in the GOP layer of field 2.

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_SourceIsLetterboxed"></a><a id="ammpeg2_sourceisletterboxed"></a><a id="AMMPEG2_SOURCEISLETTERBOXED"></a><dl>
<dt><b>AMMPEG2_SourceIsLetterboxed</b></dt>
<dt>0x00000008</dt>
</dl>
</td>
<td width="60%">
If set, indicates that black bars have been encoded in the top and bottom of the video. 

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_FilmCameraMode"></a><a id="ammpeg2_filmcameramode"></a><a id="AMMPEG2_FILMCAMERAMODE"></a><dl>
<dt><b>AMMPEG2_FilmCameraMode</b></dt>
<dt>0x00000010</dt>
</dl>
</td>
<td width="60%">
If set, indicates "film mode" used for the 625/50 (line/field) content. If cleared, indicates that "camera mode" was used.

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_LetterboxAnalogOut"></a><a id="ammpeg2_letterboxanalogout"></a><a id="AMMPEG2_LETTERBOXANALOGOUT"></a><dl>
<dt><b>AMMPEG2_LetterboxAnalogOut</b></dt>
<dt>0x00000020</dt>
</dl>
</td>
<td width="60%">
If set and this stream is sent to an analog output, it should be letterboxed. Streams sent to VGA should be letterboxed only by renderers.

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_DSS_UserData"></a><a id="ammpeg2_dss_userdata"></a><a id="AMMPEG2_DSS_USERDATA"></a><dl>
<dt><b>AMMPEG2_DSS_UserData</b></dt>
<dt>0x00000040</dt>
</dl>
</td>
<td width="60%">
If set, the MPEG-2 decoder must process DSS style user data. 

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_DVB_UserData"></a><a id="ammpeg2_dvb_userdata"></a><a id="AMMPEG2_DVB_USERDATA"></a><dl>
<dt><b>AMMPEG2_DVB_UserData</b></dt>
<dt>0x00000080</dt>
</dl>
</td>
<td width="60%">
If set, the MPEG-2 decoder must process DVB style user data. 

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_27MhzTimebase"></a><a id="ammpeg2_27mhztimebase"></a><a id="AMMPEG2_27MHZTIMEBASE"></a><dl>
<dt><b>AMMPEG2_27MhzTimebase</b></dt>
<dt>0x00000100</dt>
</dl>
</td>
<td width="60%">
If set, the PTS, DTS timestamps advance at 27MHz rather than 90KHz. 

</td>
</tr>
<tr>
<td width="40%"><a id="AMMPEG2_WidescreenAnalogOut"></a><a id="ammpeg2_widescreenanalogout"></a><a id="AMMPEG2_WIDESCREENANALOGOUT"></a><dl>
<dt><b>AMMPEG2_WidescreenAnalogOut</b></dt>
<dt>0x00000200</dt>
</dl>
</td>
<td width="60%">
If set and this stream is sent to an analog output, it should  be in widescreen format (4x3 content should be centered on a 16x9 output). Streams sent to VGA should be widescreened only by renderers. 


</td>
</tr>
</table>
 

Set undefined flags to zero or connection will be rejected. For more information on how to use these flags, see <a href="https://msdn.microsoft.com/c7ae0137-0d02-46da-9532-738d805e327d">MPEG Decoder Preprocessing Transformations</a>.


### -field dwSequenceHeader

Start of an array that contains the sequence header, including quantization matrices and the sequence extension, if required. This field is typed as <b>DWORD</b> array to enforce 32-bit alignment. The size of the array, in bytes, is given in the <b>cbSequenceHeader</b> member.
          


## -remarks



The <a href="https://msdn.microsoft.com/153c08a8-d32c-4e9d-9da9-b915eb172327">BITMAPINFOHEADER</a> structure contained in the <a href="https://msdn.microsoft.com/en-us/library/Dd407326(v=VS.85).aspx">VIDEOINFOHEADER2</a> structure (<b>hdr</b>) cannot be followed by any pallette entries or color masks, because this structure is immediately followed by the <b>dwStartTimeCode</b> member.




## -see-also




<a href="https://msdn.microsoft.com/378f6f43-5c05-4ae4-be24-956f9fc0cacf">DirectShow Structures</a>
 

 
