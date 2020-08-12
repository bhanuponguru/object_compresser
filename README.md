# object_compresser
## features
* convert's objects like string, list, your custom class object to bytes.
* it also compresses converted bytes using bz2
* if you think that converted data is use full some where in another script, then you can also write that encripted and compressed data to a file!
* in case if you write the data in to a file, you can load that data using that file in this module. please note: it is very very hard to figure out the data by opening the saved file with notepad. if you do, you will see unnoying code. that is bytes code. you can again load that data using this module. if your a good developer or know python bit well, you can load the data, but in case of this module users, i am saying you can load using this module also. please note: you can load data saved from this module only. or you can also load if you do all the manuall process done in this module. as this module is open source, if your a good developer, you can look at this.

## changelog
* v0.0.0
    * this is the first version!
## usage
usage is symple. just type the following example code. please observe commenting provided in example code. every thing is covered in one example. for more info, see help('object_compresser') on python interpreter  
#-import the module  
import object_compresser  
#create a new data object  
data=object_compresser.data  
#just compress a string says hello  
x=data.compress('hello')  
#now, let's save this produced bytes to a file  
data.save('test.txt', x) #first parameter is filename, and second parameter is bytes object  
#now, instead of creating and saving manually, lets save that directly.  
data.compress_and_save('hello', 'test.txt') #first parameter is data object and second parameter is filename.  
#now, lets learn loading and decompressing the bytes data created by this module.  
y=data.load('test.txt') #this return's the bytes like object created by this module while saving  
#now lets decompress the retrieved data  
data.decompress(y) #this will return original object which we tryed to compress and save on first.  
#now lets learn how to load and decompress it self.  
data.load_and_decompress('test.txt') #first parameter is file name that we saved our bytes in. this directly return's the data object.  
i tryed to cover every thing here. if you have more doubts, contact me or type help('object_compresser') on python interpreter. assuming you installed our module.  
note: this is beta version. so bugs mey occur. in that case let me know by one of the contact info i provide at the end.
## helping in development
if your a developer and wan't to help me, you can contact me to do so and we can together make it.
## License:

Copyright (C) 2020  TBC studios.
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Lesser General Public License as published by
the Free Software Foundation, version 3 of the License.
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Lesser General Public License for more details.
You should have received a copy of the GNU Lesser General Public License
along with this program.  If not, see https://github.com/bhanuponguru/object_compresser/blob/master/LICENSE.html.

## contact info
email: bhanuponguru@gmail.com  
twitter: @bhanuponguru  
skype: https://join.skype.com/invite/iA8MUgqF2bup  
facebook: bhanuponguru  
please note: i will bee active on skype always. i will parshally check other alternatives.  
so if you have skype, i suggest you to contact me on skype. if you don't have skype. then it's ok. i will try my level best to respond.