---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Viewer"
product_tag: "viewer"
platform: "Node.js"
platform_tag: "nodejs"

############################# Head ############################
head_title: "Node.js Document Viewer Cloud SDK | Render PDF Word Excel Visio HTML"
head_description: "Document viewer Node.js Cloud SDK and REST APIs to render all popular business document formats in HTML, image, PDF or its original format."

############################# Header ############################
title: "View Documents Online via Node.js SDK"
description: "Node.js APIs to view documents of popular file formats in HTML, image, PDF or in original format. Render whole file, page wise or range wise."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Viewer Cloud SDK for Node.js"
        image: "/sdk/272x272/groupdocs_viewer-for-node.webp"
        product: "GroupDocs.Viewer"
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
            - link: "https://docs.groupdocs.cloud/viewer/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-viewer-cloud/groupdocs-viewer-cloud-node"
        link_learn: "https://docs.groupdocs.cloud/viewer/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Viewer Cloud is a true REST API that gives the complete freedom of platform & programming language whereas GroupDocs.Viewer Cloud SDK for Node.js is built as a layer on the top of GroupDocs.Viewer Cloud REST API, allowing a higher level of abstraction so that you don't need to know the REST API to use this SDK.

      GroupDocs.Viewer Cloud API allows you to seamlessly enhance your application with the capability to render a number of document formats with the ability to view a specific document in HTML, image, PDF or its original format. You also get the flexibility to render the whole document, page by page or custom range of pages. GroupDocs.Viewer Cloud SDK for Node.js has been developed to help you integrate all these features in your Node.js application without any hassle.


    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          GroupDocs.Viewer Cloud SDK for Node.js has the following requirements.

        right:
          enable: true
          icon: "fas fa-cubes"
          title: "npm"
          content: |
            
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Viewer Cloud SDK for Node.js supports a number of document formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office"
              content: |
                * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel:** XLS, XLSX, XLSM, XLSB, XLTX, XLTM
                * **PowerPoint:**  PPT, PPTX, PPS, PPSX, PPSM, PPTM, POTX, POTM
                * **Visio:** VSD, VSDX, VSDM, VST, VSTX, VSTM, VSS, VSSX, VSSM, VDX, VSX, VTX, VDW
                * **Project:** MPP, MPT
                * **Outlook:** MSG, EML, PST, OST
                * **OneNote:** ONE

            

        right:
          enable: true
          table:
            # table loop
            - title: "Images, Graphics & Diagrams"
              content: |
                * **OpenDocument:** ODT, OTT, ODS, OTS, ODP, OTP, ODG
                * **Fixed Layout:** PDF, XPS
                * **eBook:** EPUB, MOBI
                * **Image Files:** BMP, GIF, ICO, JPG, JPEG, PNG, PSD, SVG, TIF, TIFF, Webp, DjVu, DNG, DCM (DICOM)
                * **JPEG2000:** JP2, J2C, J2K, JPF, JPX, JPM
                * **CAD:** DGN, DWF, DWG, DXF, IFC, STL
                * **Markup:** HTML, MHT, MHTML, XML
                * **Metafile:** WMF, EMF, CGM
                * **Apple Mail:** EMLX
                * **PostScript:** PS, EPS
                * **Other:** RTF, TXT, TEX, CSV, TSV, PCL
                
      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment, you can still easily get started with GroupDocs.Viewer REST API while using your favorite language & platform.
        
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
    title: "Advanced Document Viewer REST API Features"

    feature:
      # feature loop
      - icon: "fab fa-html5"
        content: "Render documents as HTML5"

      # feature loop
      - icon: "fas fa-images"
        content: "Render documents as Image"

      # feature loop
      - icon: "fas fa-file-alt"
        content: "Rotate, reorder & watermark pages"
      
      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render documents as PDF"

      # feature loop
      - icon: "fas fa-paperclip"
        content: "Render document attachments"

      # feature loop
      - icon: "fas fa-lock"
        content: "APIs are secured and require authentication"

     

      

    more_feature:
      # more_feature_loop
      - title: "Quickly Get Started with Document Viewing REST API"
        content: |
          Get started quickly using GroupDocs.Viewer Cloud REST API with the GroupDocs.Viewer Cloud SDK for Node.js. It facilitates the users and speeds up the development of their applications written in Node.js while taking care of a lot of low-level details of making requests and handling responses and lets the users focus on writing code specific to their particular project.   
      # more_feature_loop
      - title: "Explore the Options for Document Presentation"
        content: |
          The cloud-based viewer API has the ability to display different document formats quickly, with just a few lines of code. Using the SDK for Node.js you can use all these features of the API to render documents as HTML, spreadsheets or images.

          Render the document as HTML - Node.js
          
          ```js
            // Get your App SID and App Key at https://dashboard.groupdocs.cloud (free registration is required).
            var viewOptions = new groupdocs_viewer_cloud_1.ViewOptions();

            var fileInfo = new groupdocs_viewer_cloud_1.FileInfo();
            fileInfo.filePath = "viewerdocs/document.dwf";
            fileInfo.password = "";
            fileInfo.storageName = myStorage;
            viewOptions.fileInfo = fileInfo;

            var renderOptions = new groupdocs_viewer_cloud_1.HtmlOptions();
            renderOptions.externalResources = true;

            viewOptions.renderOptions = renderOptions;
            var request = new groupdocs_viewer_cloud_1.CreateViewRequest(viewOptions);

            viewerApi.createView(request)
                .then(function (response) {
                    console.log(response);
                });
          ```
      # more_feature_loop
      - title: "Easy Customization Options"
        content: "GroupDocs.Viewer Cloud SDK is 100% tested and out of the box running. The SDK is open source and has an MIT license. You can use it, and even customize it for absolutely free of charge."

      
       
       

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Viewer Cloud also offers individual document rendering SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_viewer-for-curl.webp"
          product: "GroupDocs.Viewer"
          platform: "cURL"
          link: "/viewer/curl/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_viewer-for-net.webp"
          product: "GroupDocs.Viewer"
          platform: ".NET"
          link: "/viewer/net/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_viewer-for-java.webp"
          product: "GroupDocs.Viewer"
          platform: "Java"
          link: "/viewer/java/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_viewer-for-php.webp"
          product: "GroupDocs.Viewer"
          platform: "PHP"
          link: "/viewer/php/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_viewer-for-python.webp"
          product: "GroupDocs.Viewer"
          platform: "Python"
          link: "/viewer/python/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Ruby"
          image: "/sdk/272x272/groupdocs_viewer-for-ruby.webp"
          product: "GroupDocs.Viewer"
          platform: "Ruby"
          link: "/viewer/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_viewer-for-node.webp"
          product: "GroupDocs.Viewer"
          platform: "Node.js"
          link: "/viewer/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Viewer Cloud SDK for Android"
          image: "/sdk/272x272/groupdocs_viewer-for-android.webp"
          product: "GroupDocs.Viewer"
          platform: "Android"
          link: "/viewer/android/"
    

############################# Back to top ###############################
back_to_top:
  enable: true
---