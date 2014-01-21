A pure java apk parser, to read encoded xml file and get apk infos, with no need for appt/dexdump binarys.

for now, the following is (partially) supported:
* resource table by ResourceTableParser
* binary xml file by BinaryXmlParser
* dex file by DexParser
* certificate by CetificateParser

the easiest way is to use the ApkParserUtils class, which contains convenient static mehods to get AndroidManifest.xml, apk meta infos, etc.


Also there is a cmd interface for direct using, just use dist/apk-parser-all.jar:
* java -jar apk-parser-all.jar -t manifest [apkfile]
* java -jar apk-parser-all.jar -t info [apkfile]

use java -jar apk-parser-all.jar -h to see more options.
