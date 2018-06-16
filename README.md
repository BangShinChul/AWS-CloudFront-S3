# AWSKRUG 구디모임 : AWS CloudFront + S3 을 이용한 CDN 서버 구축
- 참고 url : 
1.  https://aws.amazon.com/blogs/startups/how-to-accelerate-your-wordpress-site-with-amazon-cloudfront/
2. http://wildpup.cafe24.com/archives/830
3. http://blog.dskim.xyz/aws/2017/06/25/aws-cloudfront-s3-connection.html
---
위 url을 참고하여 S3 스토리지를 만들고 이미지를 업로드 한 뒤<br>
ClounFront를 만들고 S3 스토리지와 연결하여 S3 스토리지를 CDN 서버로 구축해보겠습니다. 
---
1. S3 Storage 만들기
	- 먼저 간단하게 cloudfront와 연결할 S3 스토리지를 생성합니다.
	- S3은 AWS에서 제공하는 클라우드 스토리지라고 생각하시면 됩니다.
	- 구글의 Google drive, MS의 OneDrive, AWS의 S3라고 생각하시면 편할 것 같습니다.

	1. S3_image 디렉토리의 스크린샷을 참고하여 S3 버킷을 생성해봅시다.
	2. 그다음 이미지 파일을 생성한 버킷안에 업로드 해봅시다.
	3. 모든 이미지가 업로드되었다면, S3에서 제공하는 링크를 통해 업로드한 파일을 브라우저에서 확인해봅시다.

2. CloudFront 만들기
	- CloudFront는 AWS에서 제공하는 CDN서비스 중 하나입니다.
	- CloudFront를 통해 간단하게 CDN 서버를 구축할 수 있습니다.
	- 우리는 S3 버킷을 CloudFront와 연결하여 S3 버킷안의 정적인 파일들(이미지, js, css 등)을 CDN서버를 통해 접근할 수 있도록 CloudFront_image 디렉토리의 스크린샷을 참고하여 만들어보겠습니다.


