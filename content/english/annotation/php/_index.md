---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Php"
platform_tag: "php"

############################# Head ############################
head_title: "PHP Document & Image Annotation Cloud SDK for PDF Word Excel Email"
head_description: "PHP Cloud SDK to annotate images and documents. Use REST APIs for PDF, image, HTML, Word, Excel, presentations, CAD & email annotation."

############################# Header ############################
title: "Let's Annotate with REST API in PHP"
description: "Annotator SDK for PHP developers allows quick, reliable and multiple types of text and image annotations with minimal code."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation Cloud SDK for PHP"
        image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-php.png"
        product: "GroupDocs.Annotation"
        platform: "PHP"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/annotation/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://github.com/groupdocs-annotation-cloud/groupdocs-annotation-cloud-php"
        link_learn: "https://docs.groupdocs.cloud/annotation/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Cloud SDK for PHP works as a handy document annotation toolkit for developers. This allows you to build data-labeling solutions in PHP that let your end-users apply various types of annotations and text markups to better collaborate via their business documents. Its cross-platform support makes it the default choice for individuals and businesses of all sorts for annotating their documents of all popular file formats. The annotation solution also works with 3rd party cloud storage providers.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          SDK requires only PHP and can run on any platform where this requirement can be met.
      
        left:
          enable: false
          icon: "fas fa-crop"
          title: "Figure Annotations"
          content: |
            
        right:
          enable: true
          icon: "fas fa-cubes"
          title: "PHP 5.5 or later"
          content: |
            
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation Cloud supports a number of document formats including almost all common business document and image file formats.



        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, RTF
                * **Excel**:  XLS, XLSX, XLSM, XLSB, CSV
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Visio**: VSD, VSDX, VSS, VST

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT, ODS, ODP
                * **Image Files**: BMP, PNG, JPG, JPEG, TIFF, TIF, GIF
                * **Fixed Layout**: PDF
                * **Web**: HTM, HTML
                * **Email**: EML
                * **CAD**: DWG, DXF


      ## TAB THREE ##
      tab_three:
        description: |
          If you do not want to use any of our SDKs or the required SDK is not available at the moment,yo u can still easily get started with GroupDocs.Annotation Cloud REST API while using your favorite language & platform.
      
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
    title: "Advanced Document Annotation REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-thumbtack"
        content: "Add/remove graphic annotations & text markups"

      # feature loop
      - icon: "fas fa-info"
        content: "Retrieve document information such as metadata"

      # feature loop
      - icon: "fas fa-asterisk"
        content: "Fetch annotation data for supported file formats"
      
      # feature loop
      - icon: "fas fa-download"
        content: "Import/export annotation list of the document"

      # feature loop
      - icon: "fas fa-file-pdf"
        content: "Render annotated document to PDF"

      # feature loop
      - icon: "fas fa-upload"
        content: "Save resultant annotated document to storage & fetch its link"

      # feature loop
      - icon: "fas fa-tachometer-alt"
        content: "Support for multiple file formats & Cross-platform compatibility"

      # feature loop
      - icon: "fas fa-eye-slash"
        content: "Apply text redaction to the slide's content"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Apply annotations to Header/Footer area in Microsoft Word documents"
    
    more_feature:
      # more_feature_loop
      - title: "Quick & Reliable Document Annotation"
        content: "GroupDocs.Annotation Cloud API provides a number of ways to deal with annotations. It not only allows retrieving annotations from documents, but also adds(exports) or remove annotations from a document and retrieves the resultant document as the stream.‎"

      # more_feature_loop
      - title: "Remove document annotations - PHP"
        content: |
          
          ```js
            //Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
            $configuration = new Configuration();
            $configuration->setAppSid($sid);
            $configuration->setAppKey($key);
            $annotationApi = new AnnotationApi($configuration);
            $request = new Requests\DeleteCleanDocumentRequest("template.pdf","SourceFiles");
            $response = $annotationApi->deleteCleanDocument($request);
          ```
      # more_feature_loop
      - title: "Robust Set of Annotation Tools"
        content: "In GroupDocs.Annotation Cloud SDK for PHP, two types of annotations are available; graphical and text-based.

        Text-based annotations, support adding text comments to selections, hiding classified text via redaction, markups to highlight text with underlines/strikethroughs, and stickynotes to be added to rich text.

        Graphical annotations, support adding notes to rectangular highlighted area, hiding confidential text or image, applying notes to a particular point within the document, dropping arrows to point to an object, drawing freehand lines and shapes, applying text-based watermarks, and distance based annotations."

      # more_feature_loop
      - title: "Easy Integration"
        content: "No installation is required on the client or server end. Just create an account at GroupDocs.Cloud to get the App SID & Key and you are ready to integrate GroupDocs.Annotation Cloud SDK into your PHP applications."

      # more_feature_loop
      - title: "Easy Customization"
        content: "Customization is quick, easy and realiable because GroupDocs.Annotation Cloud SDK for PHP is open source, has an MIT license, thouroughly tested and out of the box running. So you can use it, and even customize it as per your requirements free of charge."
      # more_feature_loop
      - title: "Interactive API Explorer"
        content: "Check our Swagger based API explorer, where you can view list of all the features that our annotation PHP API offers you. Moreover, you can try out any feature right in your browser by providing desired parameters. Please visit our Interactive API Explorer now."
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation Cloud Product Family also includes SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for cURL"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-curl.png"
          product: "GroupDocs.Annotation"
          platform: "cURL"
          link: "/annotation/curl/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-net.png"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for PHP"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-php.png"
          product: "GroupDocs.Annotation"
          platform: "PHP"
          link: "/annotation/php/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Python"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-python.png"
          product: "GroupDocs.Annotation"
          platform: "Python"
          link: "/annotation/python/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Ruby"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-ruby.png"
          product: "GroupDocs.Annotation"
          platform: "Ruby"
          link: "/annotation/ruby/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Node.js"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-node.png"
          product: "GroupDocs.Annotation"
          platform: "Node.js"
          link: "/annotation/nodejs/"

        # solution loop
        - img_alt: "GroupDocs.Annotation Cloud SDK for Android"
          image: "https://www.groupdocs.cloud/templates/groupdocscloud/images/sdk/272x272/groupdocs_annotation-for-android.png"
          product: "GroupDocs.Annotation"
          platform: "Android"
          link: "/annotation/android/"

############################# Back to top ###############################
back_to_top:
  enable: true
---