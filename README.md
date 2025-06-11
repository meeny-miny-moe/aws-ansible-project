# aws-ansible-project
aws-ansible-project

프로젝트 개요

이 프로젝트는 AWS 클라우드 환경에서 Ansible을 활용한 인프라 자동화 및 애플리케이션 배포를 목표로 합니다. YAML 기반의 플레이북을 통해 EC2 인스턴스 설정, IAM 권한 구성, CodeDeploy를 통한 서비스 배포를 자동화하며, DevOps 파이프라인을 간편하고 반복 가능하게 구축할 수 있습니다.

주요 기능

Ansible을 통한 인프라 구성 자동화


EC2 인스턴스, IAM 정책, CodeDeploy 역할 자동 설정


Docker 기반 애플리케이션 배포 (선택적 확장 가능)


AWS S3, CodeDeploy, GitHub 연동


디렉토리 구조

aws-ansible-project/

├── site.yml                # 메인 플레이북

├── aws_vars.yml            # AWS 설정 변수

├── sobin.yml, sumin.yml    # 사용자 정의 플레이북

├── code_deploy_ec2/        # EC2 인프라 관련 롤

├── code_deploy_service/    # CodeDeploy 설정 롤

├── test.yml                # 테스트용 플레이북


사용 기술

DevOps & Automation: Ansible, YAML

AWS: EC2, IAM, S3, CodeDeploy

기타: GitHub, Bash 스크립트, JSON 정책 문서

실행 방법
aws_vars.yml 파일에서 AWS 자격 정보 및 리소스 변수 설정

다음 명령어로 인프라 구성 실행 : ansible-playbook site.yml

배포 및 테스트 플레이북: ansible-playbook test.yml

사전 요구사항

AWS CLI 설정 및 IAM 권한

Ansible 설치 환경

GitHub 및 CodeDeploy 연동 준비

기여자

@meeny-miny-moe (https://github.com/meeny-miny-moe)

