---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Conversion"
product_tag: "conversion"
platform: "Node.js"
platform_tag: "node"

############################# Head ############################
head_title: "Node.js Document Converter Cloud SDK for PDF Word Excel HTML Email"
head_description: "Node.js Cloud SDK for images and documents conversion. Use REST APIs to convert HTML, Word, Excel, PPTX, Visio, Project, PDF & email file formats."

############################# Header ############################
title: "Node.js Cloud SDK for Document Conversion"
description: "Enhance your tools & applications with document and image conversion features using REST API and Node.js Cloud SDK."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Conversion Cloud SDK for Node.js"
        image: "/sdk/272x272/groupdocs_conversion-for-node.webp"
        product: "GroupDocs.Conversion"
        platform: "Node.js"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "https://docs.groupdocs.cloud/conversion/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-conversion-cloud/groupdocs-conversion-cloud-node"
        link_learn: "https://docs.groupdocs.cloud/conversion/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      The GroupDocs.Conversion Cloud SDK for Node.js has been developed to help you get started with our document conversion REST API, which lets you seamlessly convert your documents to any format you need. With this single API, you can convert back and forth between over 50 types of documents and images, including all Microsoft Office and OpenDocument file formats, PDF documents, HTML, CAD, raster images and many more. 
    tabs:
      enable: true   
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Conversion Cloud for Node.js has following SDK Requirements:

        right:
          enable: true
          icon: "fas fa-cubes"
          title: "Node.js 4.8.7 or higher"
          content: |
            

      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Conversion Cloud converts back and forth between a variety of documents and images.

        left:
          enable: true
          table:
            # table loop
            - title: "Convert From:"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP, OTS, ODG
                * **Microsoft Excel**: XLS, XLSX, XLSM, XLSB, XLT, XLAM
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX, POT
                * **Visio???**: VSD, VDX, VSS, VSX, VST, VTX, VSDX, VDW, VSSX, VSTX, VSDM, VSTM, VSSM
                * **Project**: MPP, MPT, MPX
                * **Microsoft OneNote**: ONE
                * **Email**: MSG, EML, EMLX
                * **Fixed Layout**: PDF, XPS
                * **Web**: HTML, MHT, MHTML
                * **AutoCAD**: DXF, DWG, DWT, STL, DWF, IFC
                * **Image files**: BMP, GIF, JPG, PNG, TIFF, multi-page TIFF, WebP, DjVu, SVG, DNG, DIB, JPC, JPEG-LS
                * **Metafile**: WMF, EMF
                * **Other**: TXT, CSV, XML, DICOM, TEX, MOBI, EPUB, ICO

        right:
          enable: true
          table:
            # table loop
            - title: "Convert To:"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP
                * **OpenDocument**:  XLS, XLSX, XLSM, XLSB, XLAM
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Metafiles**: WMF, EMF
                * **Image Files**: BMP, GIF, JPG, PNG, TIFF, multi-page TIFF, WebP, SVG, DNG, PSD
                * **Other**: PDF, EPUB, TXT, HTML???

      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Conversion Cloud API while using your favorite language & platform.
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "Advanced Document Conversion API Features"

    feature:
      # feature loop
      - icon: "fas fa-retweet"
        content: "Convert across all common formats"

      # feature loop
      - icon: "fas fa-star"
        content: "Convert page by page or custom range of pages"

      # feature loop
      - icon: "fas fa-copy"
        content: "Watermark pages"
      
      # feature loop
      - icon: "fas fa-star"
        content: "Get high quality output files"

      # feature loop
      - icon: "fas fa-shield-alt"
        content: "Password protect output document"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"


      

    more_feature:
      # more_feature_loop
      - title: "Convert a Multitude of Document Formats"
        content: |
          GroupDocs.Conversion REST API has the capability to perform conversion on a number of document formats. All the file formats supported by the API can be obtained using the code mentioned below:
      
      # more_feature_loop
      - title: "Get a list of supported document formats - Node.js"
        content: |
          ```js
          // Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).

          // Load module and set credentials
          var GroupDocs = require('groupdocs-conversion-cloud');
          var appSid = "XXXXXXXX";
          var appKey = "XXXXXXXX";

          // Retrieve all the supported file formats
          // construct ConversionApi
          var conversionApi = GroupDocs.ConversionApi.fromKeys(appSid, appKey);
          var request = new GroupDocs.GetSupportedConversionTypesRequest();
          conversionApi.getSupportedConversionTypes(request)
              .then(function (response) {
                  console.log("== Supported File Formats ==");
                  response.forEach(function (format) {
                      console.log(format.sourceFormat + " - to - " + format.targetFormats + "\n");
                  });
              })
              .catch(function (error) {
                  console.log("Error: " + error.message);
              });
          ```

      # more_feature_loop
      - title: "Get Started in No Time"
        content: "GroupDocs.Conversion Cloud API is completely independent of your operating system, database system or development language. You can use any language and platform that supports HTTP to interact with our API. However, manually writing client code can be difficult, error-prone and time-consuming. Therefore, we have provided and support API SDKs in many development languages in order to make it easier to integrate with us. If you use SDK, it hides the REST API calls and lets you use GroupDocs.Conversion Cloud API features in a native way for your preferred language. "

      # more_feature_loop
      - title: "Security and Authentication"
        content: "The GroupDocs.Conversion Cloud API is secured and requires authentication. Users need to register at GroupDocs Cloud and get their app access key ID (appSID) and app secret access key. Authenticated requests require a signature and AppSID query parameters or OAuth 2.0 athrorization header."
      
      # more_feature_loop
      - title: "Easy Customization"
        content: "GroupDocs.Conversion Cloud SDK is 100% tested and out of the box running. The SDK is open source and has an MIT license. You can use it, and even customize it for absolutely free of charge."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Conversion Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_conversion-for-curl.webp"
          product: "GroupDocs.Conversion"
          platform: "cURL"
          link: "/conversion/curl/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_conversion-for-net.webp"
          product: "GroupDocs.Conversion"
          platform: ".NET"
          link: "/conversion/net/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_conversion-for-java.webp"
          product: "GroupDocs.Conversion"
          platform: "Java"
          link: "/conversion/java/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_conversion-for-php.webp"
          product: "GroupDocs.Conversion"
          platform: "PHP"
          link: "/conversion/php/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_conversion-for-python.webp"
          product: "GroupDocs.Conversion"
          platform: "Python"
          link: "/conversion/python/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_conversion-for-ruby.webp"
          product: "GroupDocs.Conversion"
          platform: "Ruby"
          link: "/conversion/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_conversion-for-node.webp"
          product: "GroupDocs.Conversion"
          platform: "Node.js"
          link: "/conversion/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Conversion Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_conversion-for-android.webp"
          product: "GroupDocs.Conversion"
          platform: "Android"
          link: "/conversion/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---