---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Comparison"
product_tag: "comparison"
platform: "Ruby"
platform_tag: "ruby"

############################# Head ############################
head_title: "Ruby Document Comparison Cloud SDK for PDF Word Excel HTML Images"
head_description: "Compare images and documents with Ruby Cloud SDK &amp; REST APIs. Compare HTML, Word, Excel, Presentations, Outlook emails, PDF &amp; image file formats."

############################# Header ############################
title: "Compare Documents via Ruby Cloud SDK"
description: "Build corporate document comparison tools using REST API. Works as a comprehensive solution for all major file formats.‎‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Comparison Cloud SDK for Ruby"
        image: "/sdk/272x272/groupdocs_comparison-for-ruby.webp"
        product: "GroupDocs.Comparison"
        platform: "Ruby"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"


            # button loop
            - link: "https://docs.groupdocs.cloud/comparison/release-notes/"
              text: "Release Notes"

            # button loop
            - link: "https://purchase.groupdocs.cloud/pricing"
              text: "Pricing"

    right:
        link_download: "https://groupdocscloud.github.io/"
        link_learn: "https://docs.groupdocs.cloud/comparison/"
        link_buy: "https://purchase.groupdocs.cloud/buy"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Comparison for Cloud is a REST API that enables your Ruby applications to fetch two ‎documents of supported file format, compare those ‎same format documents and find differences ‎between them. The SDK allows you to make a resultant file and enables you to ‎accept or reject the ‎retrieved changes. Our Document Comparison SDK allows easy integration ‎into your existing Ruby ‎applications, to empower your end-users to compare documents, spreadsheets, ‎presentations, ‎Microsoft Visio diagrams, emails, and files of many other formats.‎‎‎
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          An overview of the features supported by the document comparison Cloud API.
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fas fa-check"
              title: "Accept retrieved changes"
              
            # table loop
            - icon: "fas fa-bookmark-o"
              title: "Document Resources"
              content: |
                * Result document
                * Stream of result
                * Images of result

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-trash-o"
              title: "Reject retrieved changes"
              
            # table loop
            - icon: "fas fa-retweet"
              title: "Changes Resources"
              content: |
                * Get changes
                * Update changes

      ## TAB TWO ##
      tab_two:
        description: |
          Document comparison Cloud API supported formats.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOT, DOTX, DOCM, DOTM, RTF
                * **Excel**: XLS, XLSX, XLSM, XLSB, XLS2003
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Outlook**: EML, EMLX, MSG

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **OpenDocument**: ODT, OTT, ODS, ODP, OTP
                * **Web**: HTM, HTML, MHTML
                        * **Fixed Layout**: PDF
                * **Image Files**: JPEG, BMP, PNG, GIF
                        * **Text**: TXT and other text formats with different extensions
                * **Others**: DJVU, DICOM, PDF, CSV


      ## TAB THREE ##
      tab_three:
        description: |
          Supported Operating Systems and Frameworks
      
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
    title: "Advanced Document Comparison REST API Features"

    feature:
      # feature loop
      - icon: "fas fa-file-o"
        content: "Compare Documents Stored at Cloud Storage"

      # feature loop
      - icon: "fas fa-desktop"
        content: "Fetch Documents of Supported File Types as File or Array of images"

      # feature loop
      - icon: "fas fa-copy"
        content: "Retrieve Resultant Document that Contains Differences among Compared Documents‎"
      
      # feature loop
      - icon: "fas fa-bullseye"
        content: "Get List of Categories, such as, TypeChanged or OnlyNumbers etc., for the Modified Content"

      # feature loop
      - icon: "fas fa-plug"
        content: "Accept/Reject Document Modifications to Save or Discard them"
      # feature loop
      - icon: "fas fa-file-o"
        content: "Return Document Modifications as a Set of Images or their Stream"
    
      # feature loop
      - icon: "fas fa-desktop"
        content: "Get Resultant Document (with Modifications) via Stream"
    
      # feature loop
      - icon: "fas fa-copy"
        content: "Fetch Document (with Comparison Result) as a Set of Images or their Stream"
    
      # feature loop
      - icon: "fas fa-bullseye"
        content: "Retrieve Resultant Document (with the Comparison Result) as a Stream‎"
  
    more_feature:
      # more_feature_loop
      - title: "Get Document Result as Images"
        content: "Using GroupDocs.Comparison Cloud API, you can compare documents and get the list of modifications ‎in the form of images. Following piece of code shows how you can compare a source and ‎a target ‎DOCX files and fetch their differences in a result.DOCX file. Later you can get the resultant DOCX file as ‎images using Ruby:‎"

      # more_feature_loop
      - title: "Get Document Result as Images using Ruby"
        content: |
          
          
          ```Ruby
          # TODO: Get your AppSID and AppKey at https://dashboard.groupdocs.cloud (free registration is required).
          # For complete examples and data files, please go to https://github.com/groupdocs-comparison-cloud/groupdocs-comparison-cloud-ruby
          # Returns images of document with the result of comparison
          # throws ApiException if the Api call fails

          def comparison_images
          
            @config = GroupDocsComparisonCloud::Configuration.new(Utils::APP_SID, Utils::APP_KEY)
            @config.api_base_url = Utils::API_BASE_URL
            @sourcefile = "source.docx"
            @targetfile = "target.docx"
            @outputfile= "result.docx"
          
            # Upload file to Cloud Storage
            upload_file(@sourcefile)
            upload_file(@targetfile)
          
            # Returns images of document with the result of comparison
            @comparison_api = GroupDocsComparisonCloud::ComparisonApi.from_config(@config)
            request = GroupDocsComparisonCloud::ComparisonImagesRequest.new(GetComparisonRequest(@sourcefile, @targetfile),@outputfile)
            response = @comparison_api.comparison_images(request)
            puts response
          puts 'completed'
          
          end
          ```
      

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Comparison Cloud also offers individual document comparison SDKs for other popular languages as listed below:"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for cURL"
          image: "/sdk/272x272/groupdocs_comparison-for-curl.webp"
          product: "GroupDocs.Comparison"
          platform: "Cloud for cURL"
          link: "/comparison/curl"
        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for .NET"
          image: "/sdk/272x272/groupdocs_comparison-for-net.webp"
          product: "GroupDocs.Comparison"
          platform: ".NET"
          link: "/comparison/net"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Java"
          image: "/sdk/272x272/groupdocs_comparison-for-java.webp"
          product: "GroupDocs.Comparison"
          platform: "Java"
          link: "/comparison/java"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for PHP"
          image: "/sdk/272x272/groupdocs_comparison-for-php.webp"
          product: "GroupDocs.Comparison"
          platform: "PHP"
          link: "/comparison/php"

        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Python"
          image: "/sdk/272x272/groupdocs_comparison-for-python.webp"
          product: "GroupDocs.Comparison"
          platform: "Python"
          link: "/comparison/python"
        # solution loop
        - img_alt: "GroupDocs.Comparison Cloud SDK for Node.js"
          image: "/sdk/272x272/groupdocs_comparison-for-node.webp"
          product: "GroupDocs.Comparison"
          platform: "Node.js"
          link: "/comparison/nodejs"

        

############################# Back to top ###############################
back_to_top:
  enable: true
---