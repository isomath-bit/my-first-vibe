# AGENTS.md

## 프로젝트 정보
- **프로젝트명**: 고교학점제 교과 성취도(미도달) 및 성적 분석 프로그램 (`my-first-vibe`)
- **목표**: 4세대 나이스 일람표 엑셀 업로드를 통한 지필·수행평가 합산, 경기도교육청(나이스) 중간석차 백분율 5등급제 산출 및 최소성취수준(40%) 미도달 학생 선별/보충지도 리포트 생성
- **사용자**: 고등학교 교과 담당 교사 및 학업성적관리 업무 담당자
- **보안 및 아키텍처**: 학생 성적 데이터의 외부 유출 방지를 위한 100% 클라이언트 사이드 브라우저 메모리 로컬 처리 (서버/DB 전송 없음)

## 프로젝트 식별자
- **GitHub Repository**: `https://github.com/isomath-bit/my-first-vibe`
- **Vercel Project**: `my-first-vibe`
- **Vercel Project ID**: `prj_dDtxLUMI7p2HHvig54f7nHFA8Omc`
- **Vercel Org ID**: `team_WUMwXXGkyUyfNO2w0akQqMuW`
- **Vercel Scope/Team**: `isomath-bit`
- **Supabase Ref**: 없음 (개인정보 보호 원칙 및 요구사항에 따라 데이터베이스 미사용)

## 검증 기준
1. **정적 파일 정합성**: `index.html` 및 로컬 SheetJS(`xlsx.full.min.js`)의 정상 서빙
2. **Git 추적 상태**: 불필요 파일 배제(.gitignore 적용), `git status --porcelain` 정리 완료
3. **GitHub 동기화**: `git log '@{u}..' --oneline` 미전송 커밋 없음
4. **Vercel 프로덕션 배포**: `vercel inspect` 결과 Ready 상태 및 실제 Production URL 확보
5. **웹 접속 및 기능 동작**: 공개 URL HTTP 200, 브라우저 콘솔 오류 없음, 3단계 UI 워크플로우 및 통계/엑셀 다운로드 정상 동작
6. **보안 점검**: `dorms-check` 스캔 수행 및 위험(Risk) 항목 0건 검증
